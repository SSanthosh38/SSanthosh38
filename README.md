import React from "react";

export default function App() {
  const projects = [
    { title: "New Web App", progress: 85 },
    { title: "Mobile App UI", progress: 40 },
    { title: "API Integration", progress: 60 },
    { title: "Admin Dashboard", progress: 90 },
  ];

  const snippets = [
    "React Hook Example",
    "Python Data Script",
    "Tailwind Component",
    "GitHub Snippet",
  ];

  return (
    <div className="min-h-screen bg-slate-100 p-6 font-sans">
      {/* HERO */}

      <div className="relative overflow-hidden rounded-3xl shadow-2xl">
        <img
          src="https://images.unsplash.com/photo-1515879218367-8466d910aaa4?auto=format&fit=crop&w=1600&q=80"
          alt=""
          className="h-[320px] w-full object-cover"
        />

        <div className="absolute inset-0 bg-slate-950/70"></div>

        <div className="absolute inset-0 flex flex-col justify-center px-10">
          <h1 className="text-5xl font-bold text-white">
            DEVELOPER PRODUCTIVITY HUB
          </h1>

          <p className="mt-4 text-slate-300 text-lg">
            Full Stack Workspace • MERN • System Design • Cloud
          </p>

          <div className="mt-6 flex gap-3">
            <span className="rounded-full bg-blue-500 px-4 py-2 text-white">
              React
            </span>

            <span className="rounded-full bg-slate-800 px-4 py-2 text-white">
              Node.js
            </span>

            <span className="rounded-full bg-slate-800 px-4 py-2 text-white">
              MongoDB
            </span>
          </div>
        </div>
      </div>

      {/* TITLE */}

      <div className="mt-8 rounded-3xl bg-white p-8 shadow-lg">
        <h2 className="text-4xl font-black text-slate-800">
          SANthosh S
        </h2>

        <p className="mt-2 text-slate-500">
          Full Stack Developer • Building Scalable Applications
        </p>
      </div>

      {/* ACTIVE PROJECTS */}

      <div className="mt-8">
        <h2 className="mb-5 text-2xl font-bold text-slate-800">
          🚀 Active Projects
        </h2>

        <div className="grid gap-5 md:grid-cols-4">
          {projects.map((project) => (
            <div
              key={project.title}
              className="overflow-hidden rounded-3xl bg-white shadow-lg transition-all duration-300 hover:-translate-y-2 hover:shadow-2xl"
            >
              <div className="h-36 bg-gradient-to-r from-slate-900 to-blue-900"></div>

              <div className="p-5">
                <h3 className="font-bold text-slate-800">
                  {project.title}
                </h3>

                <p className="mt-2 text-sm text-slate-500">
                  Progress {project.progress}%
                </p>

                <div className="mt-3 h-3 rounded-full bg-slate-200">
                  <div
                    className="h-3 rounded-full bg-blue-500"
                    style={{
                      width: `${project.progress}%`,
                    }}
                  />
                </div>
              </div>
            </div>
          ))}
        </div>
      </div>

      {/* DAILY STANDUP */}

      <div className="mt-8">
        <h2 className="mb-5 text-2xl font-bold text-slate-800">
          📋 Daily Standup
        </h2>

        <div className="grid gap-4 md:grid-cols-4">
          <div className="rounded-3xl bg-white p-6 shadow-lg">
            <h3 className="font-bold">Today's Focus</h3>

            <ul className="mt-3 text-slate-600">
              <li>✔ Dashboard UI</li>
              <li>✔ API Integration</li>
              <li>✔ Bug Fixes</li>
            </ul>
          </div>

          <div className="rounded-3xl bg-white p-6 shadow-lg">
            <h3 className="font-bold">Completed</h3>

            <ul className="mt-3 text-slate-600">
              <li>✔ Authentication</li>
              <li>✔ Database Setup</li>
            </ul>
          </div>

          <div className="rounded-3xl bg-white p-6 shadow-lg">
            <h3 className="font-bold">Blockers</h3>

            <ul className="mt-3 text-slate-600">
              <li>⚠ AWS Deployment</li>
            </ul>
          </div>

          <div className="rounded-3xl bg-white p-6 shadow-lg">
            <h3 className="font-bold">Next Steps</h3>

            <ul className="mt-3 text-slate-600">
              <li>➡ CI/CD</li>
              <li>➡ Docker</li>
            </ul>
          </div>
        </div>
      </div>

      {/* SNIPPETS */}

      <div className="mt-8">
        <h2 className="mb-5 text-2xl font-bold text-slate-800">
          💻 Code Snippet Library
        </h2>

        <div className="grid gap-5 md:grid-cols-4">
          {snippets.map((snippet) => (
            <div
              key={snippet}
              className="rounded-3xl bg-white p-6 shadow-lg transition-all hover:-translate-y-2 hover:shadow-2xl"
            >
              <div className="mb-4 h-16 rounded-2xl bg-slate-100"></div>

              <h3 className="font-semibold text-slate-800">
                {snippet}
              </h3>
            </div>
          ))}
        </div>
      </div>

      {/* RESOURCES */}

      <div className="mt-8 grid gap-6 md:grid-cols-2">
        <div className="rounded-3xl bg-white p-6 shadow-lg">
          <h2 className="mb-4 text-xl font-bold">
            📚 Learning Resources
          </h2>

          <ul className="space-y-2 text-slate-600">
            <li>• System Design Docs</li>
            <li>• AWS Best Practices</li>
            <li>• Docker Handbook</li>
            <li>• React Patterns</li>
            <li>• Node.js Scaling</li>
          </ul>
        </div>

        <div className="rounded-3xl bg-white p-6 shadow-lg">
          <h2 className="mb-4 text-xl font-bold">
            📈 GitHub Activity
          </h2>

          <ul className="space-y-2 text-slate-600">
            <li>Updated README.md</li>
            <li>Merged Feature Branch</li>
            <li>Fixed Authentication</li>
            <li>Added Dashboard UI</li>
            <li>Optimized API Routes</li>
          </ul>
        </div>
      </div>

      {/* FOOTER */}

      <div className="mt-10 rounded-3xl bg-slate-900 p-8 text-center text-white shadow-2xl">
        <h2 className="text-3xl font-bold">
          Building Products, Not Just Projects
        </h2>

        <p className="mt-3 text-slate-400">
          MERN • Cloud • System Design • Open Source
        </p>
      </div>
    </div>
  );
}
