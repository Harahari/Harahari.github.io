import React, { useState, useEffect } from 'react';
import { Github, Linkedin, Twitter } from 'lucide-react';

const AcademicPortfolio = () => {
  const [isNavHidden, setIsNavHidden] = useState(false);
  const [lastScroll, setLastScroll] = useState(0);

  useEffect(() => {
    const handleScroll = () => {
      const currentScroll = window.pageYOffset;
      
      if (currentScroll <= 0) {
        setIsNavHidden(false);
        return;
      }
      
      if (currentScroll > lastScroll && !isNavHidden) {
        setIsNavHidden(true);
      } else if (currentScroll < lastScroll && isNavHidden) {
        setIsNavHidden(false);
      }
      
      setLastScroll(currentScroll);
    };

    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  }, [lastScroll, isNavHidden]);

  const smoothScroll = (e) => {
    const targetId = e.target.getAttribute('href');
    const targetElement = document.querySelector(targetId);
    if (targetElement) {
      targetElement.scrollIntoView({ behavior: 'smooth' });
    }
  };

  return (
    <div className="font-sans text-gray-800">
      <nav 
        className={`fixed top-0 w-full bg-white/95 backdrop-blur-md z-50 py-4 transition-transform duration-300 ${
          isNavHidden ? '-translate-y-full' : ''
        }`}
      >
        <div className="max-w-4xl mx-auto px-8 flex justify-between items-center">
          <div className="font-bold text-xl">AK</div>
          <div className="space-x-6">
            <a href="#about" onClick={smoothScroll} className="hover:text-blue-500 relative group">
              About
              <span className="absolute bottom--2 left-0 w-0 h-0.5 bg-blue-500 transition-all group-hover:w-full"></span>
            </a>
            <a href="#publications" onClick={smoothScroll} className="hover:text-blue-500 relative group">
              Publications
              <span className="absolute bottom--2 left-0 w-0 h-0.5 bg-blue-500 transition-all group-hover:w-full"></span>
            </a>
            <a href="#projects" onClick={smoothScroll} className="hover:text-blue-500 relative group">
              Projects
              <span className="absolute bottom--2 left-0 w-0 h-0.5 bg-blue-500 transition-all group-hover:w-full"></span>
            </a>
            <a href="#contact" onClick={smoothScroll} className="hover:text-blue-500 relative group">
              Contact
              <span className="absolute bottom--2 left-0 w-0 h-0.5 bg-blue-500 transition-all group-hover:w-full"></span>
            </a>
          </div>
        </div>
      </nav>

      <div className="max-w-4xl mx-auto px-8">
        <section className="min-h-screen flex items-center py-16">
          <div className="flex items-center animate-fadeIn">
            <img 
              src="/api/placeholder/200/200" 
              alt="Akhil Krishnan" 
              className="w-48 h-48 rounded-full object-cover border-4 border-blue-500 mr-12"
            />
            <div>
              <h1 className="text-4xl font-bold mb-4">Akhil Krishnan</h1>
              <div className="text-xl text-gray-600 mb-4">
                PhD Student in Computer Science
              </div>
              <p className="text-lg max-w-xl mb-6">
                I'm a computer science researcher at University Name, focusing on computer vision 
                and machine learning. My work explores the intersection of 3D scene understanding 
                and visual reasoning.
              </p>
              <div className="space-x-4">
                <a 
                  href="#publications" 
                  onClick={smoothScroll}
                  className="px-4 py-2 border border-blue-500 text-blue-500 rounded hover:bg-blue-500 hover:text-white transition"
                >
                  View Publications
                </a>
                <a 
                  href="#contact" 
                  onClick={smoothScroll}
                  className="px-4 py-2 border border-blue-500 text-blue-500 rounded hover:bg-blue-500 hover:text-white transition"
                >
                  Get in Touch
                </a>
              </div>
            </div>
          </div>
        </section>

        <section id="publications" className="py-16">
          <h2 className="text-3xl font-bold mb-8">Selected Publications</h2>
          <div className="space-y-6">
            <div className="border border-gray-200 p-6 rounded-lg hover:shadow-md transition">
              <h3 className="text-xl text-blue-500 mb-2">
                A Novel Approach to Something Interesting
              </h3>
              <div className="text-gray-600 mb-2">
                Akhil Krishnan, Coauthor One, Coauthor Two
              </div>
              <div className="italic text-gray-600 mb-4">
                CVPR 2024
              </div>
              <div className="space-x-4">
                <a href="#" className="text-blue-500 border border-blue-500 px-3 py-1 rounded hover:bg-blue-500 hover:text-white">
                  Paper
                </a>
                <a href="#" className="text-blue-500 border border-blue-500 px-3 py-1 rounded hover:bg-blue-500 hover:text-white">
                  Code
                </a>
              </div>
            </div>
          </div>
        </section>

        <section id="projects" className="py-16">
          <h2 className="text-3xl font-bold mb-8">Featured Projects</h2>
          <div className="grid md:grid-cols-2 gap-6">
            <div className="border border-gray-200 rounded-lg overflow-hidden hover:shadow-md transition">
              <img 
                src="/api/placeholder/400/320" 
                alt="Project 1" 
                className="w-full h-48 object-cover"
              />
              <div className="p-6">
                <h3 className="text-xl font-semibold mb-2">Project Name</h3>
                <p className="text-gray-600 mb-4">
                  Brief description of the project and its key findings or impact.
                </p>
                <div className="space-x-4">
                  <a href="#" className="text-blue-500 border border-blue-500 px-3 py-1 rounded hover:bg-blue-500 hover:text-white">
                    Demo
                  </a>
                  <a href="#" className="text-blue-500 border border-blue-500 px-3 py-1 rounded hover:bg-blue-500 hover:text-white">
                    Code
                  </a>
                </div>
              </div>
            </div>
          </div>
        </section>

        <section id="contact" className="py-16 text-center">
          <h2 className="text-3xl font-bold mb-4">Get in Touch</h2>
          <p className="mb-2">Feel free to reach out for collaborations or questions.</p>
          <p className="mb-6">akhil.krishnan@university.edu</p>
          <div className="flex justify-center space-x-6">
            <a href="#" className="text-gray-600 hover:text-blue-500">
              <Github size={24} />
            </a>
            <a href="#" className="text-gray-600 hover:text-blue-500">
              <Twitter size={24} />
            </a>
            <a href="#" className="text-gray-600 hover:text-blue-500">
              <Linkedin size={24} />
            </a>
          </div>
        </section>
      </div>
    </div>
  );
};

export default AcademicPortfolio;
