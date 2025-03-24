import React from 'react';
import { 
  Rocket, 
  Ghost, 
  Moon, 
  Star, 
  Cpu, 
  Target, 
  GitBranch,
  BookOpenText,
  MessageCircle,
  ExternalLink
} from 'lucide-react';

const JapaneseThemeGithubProfile = () => {
  const projects = [
    {
      name: 'Crop Prediction AI',
      description: 'Neural Network-powered crop recommendation system',
      icon: <Target className="text-pink-400" />,
      link: 'https://github.com/yourusername/crop-prediction-ai',
      color: 'from-pink-300 to-rose-500',
      technologies: ['PyTorch', 'Neural Networks', 'Data Analysis']
    },
    {
      name: 'Medical AI Chatbot',
      description: 'Multilingual edge-computing medical assistant',
      icon: <MessageCircle className="text-lavender-400" />,
      link: 'https://github.com/yourusername/medical-ai-chatbot',
      color: 'from-lavender-300 to-purple-500',
      technologies: ['Mistral-7B', 'Whisper ASR', 'Raspberry Pi']
    },
    {
      name: 'Student Open-Ended Chatbot',
      description: 'Advanced conversational AI for academic interactions',
      icon: <Ghost className="text-sakura-400" />,
      link: 'https://github.com/yourusername/student-chatbot',
      color: 'from-sakura-300 to-pink-500',
      technologies: ['RAG', 'LangChain', 'GPT-Neo']
    },
    {
      name: 'ANPR Security System',
      description: 'Intelligent license plate recognition system',
      icon: <GitBranch className="text-sky-400" />,
      link: 'https://github.com/yourusername/anpr-security-system',
      color: 'from-sky-300 to-blue-500',
      technologies: ['YOLO', 'OpenCV', 'Object Detection']
    },
    {
      name: 'Traffic Management System',
      description: 'AI-driven traffic optimization using computer vision',
      icon: <Rocket className="text-cherry-400" />,
      link: 'https://github.com/yourusername/traffic-management-system',
      color: 'from-cherry-300 to-red-500',
      technologies: ['OpenCV', 'YOLO', 'Raspberry Pi']
    }
  ];

  const techSkills = [
    'Python', 'TensorFlow', 'PyTorch', 'OpenCV', 
    'LangChain', 'Computer Vision', 'Edge AI', 
    'RAG Chatbots', 'YOLO', 'ROS 2'
  ];

  return (
    <div className="min-h-screen bg-gradient-to-br from-white via-pink-50 to-white text-gray-800 p-8 overflow-hidden relative">
      {/* Cherry Blossom Background */}
      <div className="fixed inset-0 z-0 opacity-30 pointer-events-none">
        {[...Array(200)].map((_, i) => (
          <div 
            key={i} 
            className="absolute bg-pink-200 rounded-full animate-blossom-float"
            style={{
              width: `${Math.random() * 4}px`,
              height: `${Math.random() * 4}px`,
              left: `${Math.random() * 100}%`,
              top: `${Math.random() * 100}%`,
              animationDelay: `${Math.random() * 10}s`
            }}
          />
        ))}
      </div>

      {/* Mountain Silhouette Background */}
      <div className="absolute bottom-0 left-0 right-0 h-64 bg-mountain-silhouette opacity-20 z-0"></div>

      <div className="relative z-10 max-w-6xl mx-auto bg-white/90 rounded-3xl shadow-2xl shadow-pink-200/50 border border-pink-100 overflow-hidden">
        {/* Header with Soft Pink Gradient */}
        <div className="relative bg-gradient-to-r from-pink-100 via-pink-200 to-pink-100 p-8 text-center overflow-hidden">
          <h1 className="relative text-5xl font-bold text-transparent bg-clip-text bg-gradient-to-r from-pink-500 to-rose-600 animate-sakura-glow">
            Prabhaharan S
          </h1>
          <p className="relative text-xl mt-2 text-pink-700 animate-soft-float">
            Innovative AI Craftsman | Machine Learning Artisan
          </p>
        </div>

        {/* Main Content with Japanese-Inspired Layout */}
        <div className="relative grid md:grid-cols-2 gap-8 p-8">
          {/* Projects Section */}
          <div>
            <h2 className="text-3xl font-semibold mb-6 border-b-2 border-pink-300 pb-2 text-pink-600">
              🌸 Innovative Projects
            </h2>
            <div className="space-y-4">
              {projects.map((project, index) => (
                <div 
                  key={index} 
                  className={`bg-gradient-to-r ${project.color} p-5 rounded-xl flex items-center hover:scale-105 transition duration-300 group relative overflow-hidden shadow-md`}
                >
                  {project.icon}
                  <div className="ml-4 flex-grow z-10">
                    <h3 className="font-bold text-lg text-white">{project.name}</h3>
                    <p className="text-sm text-white/80">{project.description}</p>
                    <div className="flex flex-wrap gap-1 mt-2">
                      {project.technologies.map((tech, techIndex) => (
                        <span 
                          key={techIndex} 
                          className="bg-white/20 text-white px-2 py-1 rounded-full text-xs"
                        >
                          {tech}
                        </span>
                      ))}
                    </div>
                  </div>
                  <a 
                    href={project.link} 
                    target="_blank" 
                    rel="noopener noreferrer"
                    className="z-20 opacity-0 group-hover:opacity-100 transition duration-300"
                  >
                    <ExternalLink className="text-white hover:text-pink-200" />
                  </a>
                </div>
              ))}
            </div>
          </div>

          {/* Skills & Education Section */}
          <div>
            <h2 className="text-3xl font-semibold mb-6 border-b-2 border-pink-300 pb-2 text-pink-600">
              🍃 Skill Garden
            </h2>
            <div className="bg-pink-50 rounded-lg p-6 border border-pink-200">
              <div className="flex flex-wrap gap-2">
                {techSkills.map((skill, index) => (
                  <span 
                    key={index} 
                    className="bg-pink-200/50 text-pink-800 px-3 py-1 rounded-full text-sm hover:bg-pink-300/60 transition"
                  >
                    {skill}
                  </span>
                ))}
              </div>
            </div>

            <div className="mt-8 bg-pink-50 rounded-lg p-6 border border-pink-200">
              <h3 className="text-2xl font-semibold mb-4 border-b border-pink-300 pb-2 text-pink-600">
                🏔️ Academic Journey
              </h3>
              <div>
                <BookOpenText className="mr-4 text-rose-500 inline-block" />
                <span className="font-bold text-gray-800">Dr. Mahalingam College of Engineering</span>
                <p className="text-pink-700">B.E in CSE (AI & ML) | CGPA: 8.2 | 2023-2027</p>
              </div>
            </div>
          </div>
        </div>

        {/* Footer with Soft Design */}
        <div className="bg-pink-100/50 p-6 text-center border-t border-pink-200">
          <p className="text-pink-700">
            📧 prabhasuresh2006@gmail.com | 🌸 GitHub: @yourusername
          </p>
        </div>
      </div>

      {/* GitHub Stats with Soft Pink Theme */}
      <div className="relative max-w-6xl mx-auto mt-8 bg-white/90 rounded-3xl p-8 border border-pink-100 shadow-lg">
        <div className="grid md:grid-cols-2 gap-8">
          <img 
            src="https://github-readme-stats.vercel.app/api?username=yourusername&theme=react&hide_border=true&bg_color=FFF0F5&title_color=FF69B4&text_color=333&icon_color=FF1493" 
            alt="GitHub Stats" 
            className="w-full rounded-lg shadow-pink-200/50 shadow-lg"
          />
          <img 
            src="https://github-readme-streak-stats.herokuapp.com/?user=yourusername&theme=react&hide_border=true&background=FFF0F5&currStreakColor=FF69B4&sideNormalAmt=333" 
            alt="GitHub Streak" 
            className="w-full rounded-lg shadow-pink-200/50 shadow-lg"
          />
        </div>
      </div>

      {/* Soft Animations and Custom Styles */}
      <style jsx global>{`
        @keyframes blossom-float {
          0%, 100% { transform: translateY(0) rotate(0deg); opacity: 0.3; }
          50% { transform: translateY(-20px) rotate(180deg); opacity: 0.6; }
        }
        @keyframes sakura-glow {
          0%, 100% { text-shadow: 0 0 5px rgba(255,105,180,0.3); }
          50% { text-shadow: 0 0 15px rgba(255,105,180,0.6); }
        }
        @keyframes soft-float {
          0%, 100% { transform: translateY(0); }
          50% { transform: translateY(-5px); }
        }
        .animate-blossom-float {
          animation: blossom-float 10s infinite;
        }
        .animate-sakura-glow {
          animation: sakura-glow 3s infinite;
        }
        .animate-soft-float {
          animation: soft-float 3s infinite;
        }
        .bg-mountain-silhouette {
          background-image: linear-gradient(rgba(255,255,255,0), rgba(255,255,255,0.1)), 
            url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 1440 320'%3E%3Cpath fill='%23FFB6C1' fill-opacity='0.2' d='M0,224L48,208C96,192,192,160,288,144C384,128,480,128,576,154.7C672,181,768,235,864,261.3C960,288,1056,288,1152,261.3C1248,235,1344,181,1392,154.7L1440,128L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z'%3E%3C/path%3E%3C/svg%3E");
          background-position: bottom;
          background-repeat: no-repeat;
          background-size: cover;
        }
      `}</style>
    </div>
  );
};

export default JapaneseThemeGithubProfile;
