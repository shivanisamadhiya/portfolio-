# portfolio-
import React from 'react';

const CyberpunkProjectCard = () => {
  // Project data based on your AI Consultation Platform
  const project = {
    codeName: "MISSION // PROJECT_AEGIS",
    title: "AI-Powered Consultation Platform",
    role: "CORE ARCHITECT",
    status: "SYSTEM OPERATIONAL",
    deployment: {
      frontend: "VERCEL_NODE_01",
      backend: "RENDER_CLUSTER_02"
    },
    techStack: ["MongoDB", "Express.js", "React.js", "Node.js", "Tailwind CSS", "ZegoCloud SDK", "Cloudinary"],
    features: [
      "Integrated ZegoCloud SDK for real-time, low-latency video conferencing networks.",
      "Engineered an intelligent AI chatbot sub-routine to automate inquiry routing.",
      "Designed full-stack secure data pipelines for real-time booking flows."
    ],
    links: {
      live: "https://vercel.com", // Replace with your actual links
      github: "https://github.com/shivani-samadhiya"
    }
  };

  // Inline clip-path style for that sharp, asymmetric Persona 5 / Star Rail UI cut
  const sharpCornerStyle = {
    clipPath: 'polygon(0 0, 100% 0, 100% calc(100% - 24px), calc(100% - 24px) 100%, 0 100%)'
  };

  const tagStyle = {
    clipPath: 'polygon(0 0, 100% 0, calc(100% - 8px) 100%, 0 100%)'
  };

  return (
    <div className="min-h-screen bg-[#08090d] flex items-center justify-center p-6 text-slate-200 font-mono select-none">
      
      {/* Container Node */}
      <div 
        style={sharpCornerStyle}
        className="relative w-full max-w-xl bg-[#11131c] border-l-4 border-t border-b border-r border-r-transparent border-t-purple-500 border-b-magenta border-l-[#ff007f] p-6 shadow-[0_0_25px_rgba(255,0,127,0.15)] transition-all duration-300 hover:shadow-[0_0_35px_rgba(255,0,127,0.3)] hover:border-t-[#ff007f] group"
      >
        {/* Neon Scanline Accent Overlay */}
        <div className="absolute top-0 left-0 w-full h-[2px] bg-gradient-to-r from-[#ff007f] via-[#8a2be2] to-transparent opacity-70 group-hover:animate-pulse" />

        {/* Top Header Row */}
        <div className="flex justify-between items-center mb-4 border-b border-slate-800 pb-3">
          <div className="flex items-center space-x-2">
            <span className="w-2 h-2 bg-[#ff007f] animate-ping rounded-full" />
            <span className="text-xs font-bold tracking-widest text-[#ff007f] uppercase">
              {project.codeName}
            </span>
          </div>
          <div className="text-[10px] bg-[#221226] text-[#df52ff] px-2 py-0.5 border border-[#df52ff]/30 uppercase font-black tracking-wider">
            {project.status}
          </div>
        </div>

        {/* Project Title */}
        <h2 className="text-2xl font-black text-white tracking-tight uppercase group-hover:text-[#ff007f] transition-colors duration-200 mb-1">
          {project.title}
        </h2>
        
        <p className="text-xs text-purple-400 font-bold tracking-wider mb-4">
          SYSTEM_ROLE: <span className="text-slate-300">{project.role}</span>
        </p>

        {/* Tech Stack Modules */}
        <div className="flex flex-wrap gap-2 mb-6">
          {project.techStack.map((tech, idx) => (
            <span 
              key={idx}
              style={tagStyle}
              className="bg-[#1a1d29] text-xs font-semibold text-cyan-400 px-3 py-1 border-l border-cyan-400 uppercase tracking-wide hover:bg-cyan-500 hover:text-black transition-colors duration-150 cursor-crosshair"
            >
              {tech}
            </span>
          ))}
        </div>

        {/* Tactical Subsystems (Features) */}
        <div className="space-y-3 mb-6">
          <p className="text-[11px] uppercase font-black tracking-widest text-slate-500">
            // SUBSYSTEM_CAPABILITIES
          </p>
          {project.features.map((feature, idx) => (
            <div key={idx} className="flex items-start space-x-2 text-sm text-slate-400">
              <span className="text-[#ff007f] font-black mt-0.5">▷</span>
              <p className="leading-relaxed">{feature}</p>
            </div>
          ))}
        </div>

        {/* Server Deploy Nodes */}
        <div className="grid grid-cols-2 gap-2 bg-[#0c0d14] p-3 border border-slate-800 text-[11px] mb-6">
          <div>
            <span className="text-slate-500 uppercase block">Host Node Alpha:</span>
            <span className="text-purple-400 font-bold">{project.deployment.frontend}</span>
          </div>
          <div>
            <span className="text-slate-500 uppercase block">Host Node Beta:</span>
            <span className="text-purple-400 font-bold">{project.deployment.backend}</span>
          </div>
        </div>

        {/* Interactive Control Links */}
        <div className="flex space-x-3 pt-2">
          <a 
            href={project.links.live}
            target="_blank"
            rel="noreferrer"
            className="flex-1 text-center bg-gradient-to-r from-[#ff007f] to-[#8a2be2] text-white font-black text-xs uppercase tracking-widest py-3 transition-transform duration-150 active:scale-95 hover:brightness-110 shadow-[0_4px_10px_rgba(255,0,127,0.3)]"
          >
            [ LAUNCH_APPLICATION ]
          </a>
          <a 
            href={project.links.github}
            target="_blank"
            rel="noreferrer"
            className="px-5 border border-slate-700 text-slate-400 hover:text-white hover:border-[#ff007f] flex items-center justify-center transition-colors duration-150"
            title="View Code Matrix"
          >
            <svg className="w-4 h-4 fill-current" viewBox="0 0 24 24">
              <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
            </svg>
          </a>
        </div>

        {/* Geometric Corner Accent Details */}
        <div className="absolute bottom-1 right-2 text-[8px] text-slate-700 font-black tracking-widest pointer-events-none">
          SYS_v8.0.26
        </div>
      </div>

    </div>
  );
};

export default CyberpunkProjectCard;
