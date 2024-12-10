import React, { useState } from 'react';
import { Home, User, Briefcase, Code, Mail } from 'lucide-react';
import { motion } from 'framer-motion';

// Main App Component
const PortfolioWebsite = () => {
  const [activeSection, setActiveSection] = useState('home');

  const sections = {
    home: <HomeSection />,
    about: <AboutSection />,
    projects: <ProjectsSection />,
    skills: <SkillsSection />,
    contact: <ContactSection />
  };

  return (
    <div className="min-h-screen bg-gradient-to-br from-gray-900 via-gray-800 to-black text-white font-sans">
      <Navigation 
        activeSection={activeSection} 
        setActiveSection={setActiveSection} 
      />
      
      <motion.div 
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        transition={{ duration: 0.5 }}
        className="container mx-auto px-4 py-16"
      >
        {sections[activeSection]}
      </motion.div>
      
      <Footer />
    </div>
  );
};

// Navigation Component
const Navigation = ({ activeSection, setActiveSection }) => {
  const navItems = [
    { icon: Home, name: 'home' },
    { icon: User, name: 'about' },
    { icon: Briefcase, name: 'projects' },
    { icon: Code, name: 'skills' },
    { icon: Mail, name: 'contact' }
  ];

  return (
    <nav className="fixed bottom-8 left-1/2 transform -translate-x-1/2 z-50">
      <div className="bg-white/20 backdrop-blur-lg rounded-full p-2 flex space-x-4">
        {navItems.map((item) => (
          <button
            key={item.name}
            onClick={() => setActiveSection(item.name)}
            className={`p-3 rounded-full transition-all duration-300 ${
              activeSection === item.name 
                ? 'bg-blue-600 text-white' 
                : 'hover:bg-white/20 text-gray-300'
            }`}
          >
            <item.icon size={24} />
          </button>
        ))}
      </div>
    </nav>
  );
};

// Home Section
const HomeSection = () => (
  <div className="min-h-screen flex items-center justify-center text-center">
    <motion.div 
      initial={{ opacity: 0, y: 50 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ duration: 0.8 }}
    >
      <h1 className="text-6xl font-bold mb-4 text-transparent bg-clip-text bg-gradient-to-r from-blue-500 to-purple-600">
        Your Name
      </h1>
      <p className="text-2xl text-gray-300 mb-8">
        Software Engineer | Web Developer | Creative Technologist
      </p>
      <div className="flex justify-center space-x-4">
        <a 
          href="#" 
          className="bg-blue-600 hover:bg-blue-700 text-white px-6 py-3 rounded-full transition duration-300"
        >
          Download CV
        </a>
        <a 
          href="#contact" 
          className="border border-white/30 text-white px-6 py-3 rounded-full hover:bg-white/10 transition duration-300"
        >
          Contact Me
        </a>
      </div>
    </motion.div>
  </div>
);

// About Section
const AboutSection = () => (
  <div className="grid md:grid-cols-2 gap-8 items-center">
    <motion.div
      initial={{ x: -50, opacity: 0 }}
      animate={{ x: 0, opacity: 1 }}
      transition={{ duration: 0.6 }}
    >
      <img 
        src="/api/placeholder/400/400" 
        alt="Profile" 
        className="rounded-2xl shadow-2xl"
      />
    </motion.div>
    <motion.div
      initial={{ x: 50, opacity: 0 }}
      animate={{ x: 0, opacity: 1 }}
      transition={{ duration: 0.6 }}
    >
      <h2 className="text-4xl font-bold mb-6 text-transparent bg-clip-text bg-gradient-to-r from-blue-500 to-purple-600">
        About Me
      </h2>
      <p className="text-gray-300 mb-4">
        I'm a passionate software engineer with expertise in web technologies, 
        machine learning, and creative coding. My mission is to build innovative 
        solutions that make a positive impact.
      </p>
      <div className="grid md:grid-cols-2 gap-4 mt-6">
        <InfoCard icon="🎓" title="Education" description="Computer Science, Tech University" />
        <InfoCard icon="💼" title="Experience" description="5+ Years in Software Development" />
      </div>
    </motion.div>
  </div>
);

// Projects Section
const ProjectsSection = () => {
  const projects = [
    { 
      name: "AI Chatbot", 
      description: "Advanced conversational AI with natural language processing",
      tech: ["React", "Python", "Machine Learning"],
      image: "/api/placeholder/300/200"
    },
    { 
      name: "E-commerce Platform", 
      description: "Scalable online marketplace with microservices architecture",
      tech: ["Node.js", "Docker", "Kubernetes"],
      image: "/api/placeholder/300/200"
    }
  ];

  return (
    <div>
      <h2 className="text-4xl font-bold text-center mb-12 text-transparent bg-clip-text bg-gradient-to-r from-blue-500 to-purple-600">
        My Projects
      </h2>
      <div className="grid md:grid-cols-2 gap-8">
        {projects.map((project, index) => (
          <motion.div
            key={index}
            initial={{ scale: 0.9, opacity: 0 }}
            animate={{ scale: 1, opacity: 1 }}
            transition={{ duration: 0.5, delay: index * 0.2 }}
            className="bg-white/10 rounded-2xl overflow-hidden shadow-2xl"
          >
            <img 
              src={project.image} 
              alt={project.name} 
              className="w-full h-48 object-cover"
            />
            <div className="p-6">
              <h3 className="text-2xl font-bold mb-3">{project.name}</h3>
              <p className="text-gray-300 mb-4">{project.description}</p>
              <div className="flex flex-wrap gap-2">
                {project.tech.map((tech, i) => (
                  <span 
                    key={i} 
                    className="bg-blue-600/20 text-blue-400 px-3 py-1 rounded-full text-sm"
                  >
                    {tech}
                  </span>
                ))}
              </div>
            </div>
          </motion.div>
        ))}
      </div>
    </div>
  );
};

// Skills Section
const SkillsSection = () => {
  const skillCategories = [
    { 
      name: "Frontend", 
      skills: ["React", "Vue", "Tailwind CSS", "Next.js"] 
    },
    { 
      name: "Backend", 
      skills: ["Node.js", "Python", "Django", "Express"] 
    },
    { 
      name: "Tools", 
      skills: ["Git", "Docker", "AWS", "Kubernetes"] 
    }
  ];

  return (
    <div>
      <h2 className="text-4xl font-bold text-center mb-12 text-transparent bg-clip-text bg-gradient-to-r from-blue-500 to-purple-600">
        My Skills
      </h2>
      <div className="grid md:grid-cols-3 gap-8">
        {skillCategories.map((category, index) => (
          <motion.div
            key={category.name}
            initial={{ y: 50, opacity: 0 }}
            animate={{ y: 0, opacity: 1 }}
            transition={{ duration: 0.5, delay: index * 0.2 }}
            className="bg-white/10 p-6 rounded-2xl"
          >
            <h3 className="text-2xl font-bold mb-4 text-blue-400">
              {category.name}
            </h3>
            <div className="flex flex-wrap gap-2">
              {category.skills.map((skill, i) => (
                <span 
                  key={i} 
                  className="bg-blue-600/20 text-blue-300 px-3 py-1 rounded-full text-sm"
                >
                  {skill}
                </span>
              ))}
            </div>
          </motion.div>
        ))}
      </div>
    </div>
  );
};

// Contact Section
const ContactSection = () => (
  <div className="max-w-lg mx-auto">
    <h2 className="text-4xl font-bold text-center mb-12 text-transparent bg-clip-text bg-gradient-to-r from-blue-500 to-purple-600">
      Contact Me
    </h2>
    <motion.form
      initial={{ opacity: 0, y: 50 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ duration: 0.5 }}
      className="bg-white/10 p-8 rounded-2xl"
    >
      <div className="mb-4">
        <label className="block text-gray-300 mb-2">Name</label>
        <input 
          type="text" 
          className="w-full bg-white/10 border border-white/20 rounded-lg p-3 focus:outline-none focus:border-blue-500"
        />
      </div>
      <div className="mb-4">
        <label className="block text-gray-300 mb-2">Email</label>
        <input 
          type="email" 
          className="w-full bg-white/10 border border-white/20 rounded-lg p-3 focus:outline-none focus:border-blue-500"
        />
      </div>
      <div className="mb-4">
        <label className="block text-gray-300 mb-2">Message</label>
        <textarea 
          rows={4} 
          className="w-full bg-white/10 border border-white/20 rounded-lg p-3 focus:outline-none focus:border-blue-500"
        />
      </div>
      <button 
        type="submit" 
        className="w-full bg-blue-600 hover:bg-blue-700 text-white py-3 rounded-lg transition duration-300"
      >
        Send Message
      </button>
    </motion.form>
  </div>
);

// Footer Component
const Footer = () => (
  <footer className="bg-white/10 py-6 text-center">
    <div className="flex justify-center space-x-6 mb-4">
      <a href="#" className="text-gray-300 hover:text-white">GitHub</a>
      <a href="#" className="text-gray-300 hover:text-white">LinkedIn</a>
      <a href="#" className="text-gray-300 hover:text-white">Twitter</a>
    </div>
    <p className="text-gray-400">© 2024 Your Name. All Rights Reserved.</p>
  </footer>
);

// Utility Component
const InfoCard = ({ icon, title, description }) => (
  <div className="bg-white/10 p-4 rounded-lg">
    <div className="text-3xl mb-2">{icon}</div>
    <h3 className="font-bold text-lg">{title}</h3>
    <p className="text-gray-400 text-sm">{description}</p>
  </div>
);

export default PortfolioWebsite;
