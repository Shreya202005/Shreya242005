import React from "react";
const techStack = [
  {
    name: "Python",
    logo: "python",
    color: "00FFFF",
    link: "https://www.python.org/",
  },
  {
    name: "JavaScript",
    logo: "javascript",
    color: "F7DF1E",
    link: "https://developer.mozilla.org/en-US/docs/Web/JavaScript",
  },
  {
    name: "React",
    logo: "react",
    color: "61DAFB",
    link: "https://reactjs.org/",
  },
  {
    name: "TailwindCSS",
    logo: "tailwindcss",
    color: "38BDF8",
    link: "https://tailwindcss.com/",
  },
  {
 name: "MongoDB",
    logo: "mongodb",
    color: "00FF00",
    link: "https://www.mongodb.com/",
  },
  {
    name: "Linux",
    logo: "linux",
    color: "FCC624",
    link: "https://www.linux.org/",
  },
  {
    name: "GitHub",
    logo: "github",
    color: "white",
    link: "https://github.com/",
  },
  {
    name: "Cloud",
    logo: "icloud",
    color: "00FFFF",
    link: "https://cloud.google.com/",
  },
];
const projects = [
  {
    title: "SecureWipe Pro",
    description: "A tool for secure data wiping and IT asset recycling.",
    link: "https://github.com/shreya242005/SecureWipe-Pro",
  },
  {
    title: "Web Application Pentesting Toolkit",
    description: "Toolkit with Flask UI to scan and test vulnerabilities.",
    link: "https://github.com/shreya242005/WebApp-Pentesting-Toolkit",
  },
  {
    title: "Cloud Security Posture Management",
    description: "Visualizing security posture for cloud infrastructure.",
    link: "https://github.com/shreya242005/Cloud-Security-Posture-Management",
  },
  {
    title: "Visualizing Threat Intelligence",
    description: "Data visualization tools for cybersecurity analysts.",
    link: "https://github.com/shreya242005/Visualizing-Intelligence-Analysis",
  },
  {
    title: "Portfolio Website",
    description: "My personal portfolio built with React & Tailwind.",
    link: "https://github.com/shreya242005/my-portfolio",
  },
  {
     title: "DoS Detection",
    description: "System for detecting and mitigating denial-of-service attacks.",
    link: "https://github.com/shreya242005/DoS-Detection",
  },
];
export default function PortfolioLanding() {
  return (
    <div className="min-h-screen bg-black text-white font-sans">
      <header className="text-center py-12 border-b border-gray-800">
        <h1 className="text-5xl font-extrabold mb-2 neon-text">
          ✨ Hi, I'm Shreya ✨
        </h1>
        <h3 className="text-xl font-light text-cyan-400">
          Cybersecurity Enthusiast | Computer Science Engineering Student
        </h3>
      </header>
      <main className="max-w-6xl mx-auto px-6 py-12 space-y-20">
        {/* About Me */}
        <section>
          <h2 className="text-3xl font-bold mb-6 neon-text">🚀 About Me</h2>
          <ul className="list-disc list-inside space-y-2 text-cyan-300 text-lg max-w-3xl mx-auto">
            <li>🔐 Exploring <strong>Cybersecurity, IoT & Cloud</strong></li>
            <li>💻 Passionate about <strong>Web Security & Ethical Hacking</strong></li>
            <li>🌱 Currently building <strong>projects with React, TailwindCSS, MongoDB</strong></li>
            <li>🎯 Goal: Create <strong>secure and impactful digital solutions</strong></li>
          </ul>
 </section>
        {/* Tech Stack */}
        <section>
          <h2 className="text-3xl font-bold mb-8 neon-text">🛠️ Tech Stack</h2>
          <div className="flex flex-wrap justify-center gap-4">
            {techStack.map(({ name, logo, color, link }) => (
              <a
                key={name}
                href={link}
                target="_blank"
                rel="noopener noreferrer"
                className="transform hover:scale-110 transition-transform"
              >
                <img
                  src={`https://img.shields.io/badge/${encodeURIComponent(
                    name
                  )}-000000?style=for-the-badge&logo=${logo}&logoColor=${color}&labelColor=111`}
                  alt={name}
                  className="h-12"
                />
              </a>
            ))}
          </div>
        </section>
   {/* Featured Projects */}
        <section>
          <h2 className="text-3xl font-bold mb-8 neon-text">📂 Featured Projects</h2>
          <div className="grid grid-cols-1 md:grid-cols-2 gap-10 max-w-5xl mx-auto">
            {projects.map(({ title, description, link }) => (
              <div
                key={title}
                className="bg-gray-900 rounded-lg p-6 border border-cyan-600 hover:border-cyan-400 transition-colors shadow-lg"
              >
                <h3 className="text-2xl font-semibold mb-2 neon-text">{title}</h3>
                <p className="mb-4 text-cyan-300">{description}</p>
                <a
                  href={link}
                  target="_blank"
                  rel="noopener noreferrer"
                  className="inline-block px-4 py-2 bg-cyan-600 hover:bg-cyan-500 rounded font-medium neon-button"
                >
                  View Project
                </a>
              </div>
            ))}
          </div>
        </section>
    {/* GitHub Stats */}
        <section>
          <h2 className="text-3xl font-bold mb-8 neon-text">📊 GitHub Stats</h2>
          <div className="flex flex-col md:flex-row justify-center gap-8">
            <img
              src="https://github-readme-stats.vercel.app/api?username=shreya242005&show_icons=true&theme=radical&hide_border=true"
              alt="GitHub Stats"
              className="max-w-md"
            />
            <img
              src="https://github-readme-streak-stats.herokuapp.com/?user=shreya242005&theme=radical&hide_border=true"
              alt="GitHub Streak"
              className="max-w-md"
            />
          </div>
        </section>
  {/* Connect With Me */}
        <section className="text-center">
          <h2 className="text-3xl font-bold mb-6 neon-text">🌐 Connect With Me</h2>
          <div className="flex justify-center gap-6">
            <a
              href="https://www.linkedin.com/in/shreya242005/"
              target="_blank"
              rel="noopener noreferrer"
              aria-label="LinkedIn"
            >
              <img
                src="https://img.shields.io/badge/LinkedIn-000000?style=for-the-badge&logo=linkedin&logoColor=0A66C2&labelColor=111"
                alt="LinkedIn"
                className="h-12"
              />
            </a>
            <a
              href="mailto:tadakalashreya@gmail.com"
              aria-label="Email"
            >
              <img
                src="https://img.shields.io/badge/Gmail-000000?style=for-the-badge&logo=gmail&logoColor=EA4335&labelColor=111"
                alt="Gmail"
                className="h-12"
              />
            </a>
 <a
              href="https://shreya242005.vercel.app/"
              target="_blank"
              rel="noopener noreferrer"
              aria-label="Portfolio"
            >
              <img
                src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white&labelColor=111"
                alt="Portfolio"
                className="h-12"
              />
            </a>
          </div>
        </section>
      </main>
      <footer className="text-center py-6 border-t border-gray-800 text-gray-600 text-sm">
        © {new Date().getFullYear()} Shreya. All rights reserved.
      </footer>
  {/* Neon text and button styles */}
      <style jsx>{`
        .neon-text {
          color: #00ffff;
          text-shadow:
            0 0 5px #00ffff,
            0 0 10px #00ffff,
            0 0 20px #00ffff,
            0 0 40px #0ff,
            0 0 80px #0ff;
        }
        .neon-button {
          box-shadow:
            0 0 5px #00ffff,
            0 0 10px #00ffff,
            0 0 20px #00ffff,
            0 0 40px #0ff,
            0 0 80px #0ff;
          transition: box-shadow 0.3s ease;
        }
        .neon-button:hover {
          box-shadow:
            0 0 10px #00ffff,
            0 0 20px #00ffff,
            0 0 40px #00ffff,
            0 0 80px #0ff,
            0 0 120px #0ff;
        }
   `}</style>
    </div>
  );
}



