export default function ThaboPortfolio() { const featuredProjects = [ { title: 'Court 4 — Native Eye Creative SA', type: 'Lead Performance', year: '2026', description: 'A dramatic acting role focused on authentic township storytelling and emotional realism.', }, { title: 'Motivational Digital Content', type: 'Creator Brand', year: '2026', description: 'Short-form inspirational content designed to motivate and connect with young audiences.', }, { title: 'Street Storytelling Concepts', type: 'Creative Writing', year: '2025', description: 'Original scripts inspired by tsotsi-style storytelling, youth culture, and township experiences.', }, ]

return ( <div className="min-h-screen bg-black text-white font-sans overflow-hidden"> {{/* Navigation */} <nav className="fixed top-0 left-0 right-0 z-50 backdrop-blur-xl bg-black/70 border-b border-zinc-900"> <div className="max-w-7xl mx-auto px-6 py-5 flex items-center justify-between"> <h1 className="text-2xl font-black tracking-widest"> THABO<span className="text-red-500">.</span> </h1>

<div className="hidden md:flex items-center gap-8 text-sm uppercase tracking-wider text-zinc-400">
        <a href="#about" className="hover:text-white transition">About</a>
        <a href="#work" className="hover:text-white transition">Portfolio</a>
        <a href="#contact" className="hover:text-white transition">Contact</a>
      </div>
    </div>
  </nav>

  {/* Hero Section */}
  <section className="relative min-h-screen flex items-center px-6 overflow-hidden">
    <div className="absolute inset-0 bg-gradient-to-br from-red-950/20 via-black to-black" />

    <div className="absolute top-20 right-10 w-72 h-72 bg-red-600/20 rounded-full blur-3xl" />
    <div className="absolute bottom-10 left-10 w-72 h-72 bg-zinc-700/20 rounded-full blur-3xl" />

    <div className="relative z-10 max-w-7xl mx-auto grid lg:grid-cols-2 gap-16 items-center w-full pt-24">
      <div>
        <p className="uppercase tracking-[0.4em] text-red-400 mb-6 text-sm font-semibold">
          South African Actor & Creative
        </p>

        <h1 className="text-6xl md:text-8xl font-black leading-none mb-8">
          THABO
          <br />
          <span className="text-zinc-500">MASILELA</span>
        </h1>

        <p className="text-xl text-zinc-300 leading-9 mb-10 max-w-2xl">
          Building a bold creative identity through acting, storytelling, and youth-driven digital content.
          Focused on cinematic performances, authentic expression, and impactful entertainment.
        </p>

        <div className="flex flex-wrap gap-5">
          <a
            href="#work"
            className="bg-red-600 hover:bg-red-700 transition px-8 py-4 rounded-2xl font-bold shadow-2xl"
          >
            View Portfolio
          </a>

          <a
            href="#contact"
            className="border border-zinc-700 hover:border-white transition px-8 py-4 rounded-2xl font-bold"
          >
            Contact Me
          </a>
        </div>
      </div>

      <div className="relative">
        <div className="bg-gradient-to-b from-zinc-900 to-black border border-zinc-800 rounded-[40px] p-10 shadow-2xl">
          <div className="aspect-[4/5] rounded-[30px] bg-zinc-950 border border-zinc-800 flex items-center justify-center text-center p-6 overflow-hidden">
            <img
              src="/mnt/data/file_00000000e1fc722f9fa7c9e946dc42fc.jpg"
              alt="Thabo Masilela"
              className="w-full h-full object-cover rounded-[24px]"
            />
            <div>
              <p className="text-red-400 uppercase tracking-[0.3em] text-sm mb-6 font-semibold">
                Official Creative Portfolio
              </p>

              <h2 className="text-5xl font-black leading-tight mb-4">
                Actor.
                <br />
                Creator.
                <br />
                Storyteller.
              </h2>

              <p className="text-zinc-400 leading-8 text-lg">
                Johannesburg-based upcoming actor creating modern African entertainment experiences.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  {/* About */}}
  <section id="about" className="px-6 py-28 max-w-7xl mx-auto grid lg:grid-cols-2 gap-16 items-center">
    <div>
      <h2 className="text-4xl font-bold mb-6">About Me</h2>

      <p className="text-zinc-300 leading-8 text-lg mb-5">
        I am a young creative from South Africa building my journey in the entertainment industry.
        My work focuses on acting, storytelling, digital content, and inspiring young people through
        authentic and relatable experiences.
      </p>

      <p className="text-zinc-400 leading-8">
        I enjoy dramatic performances, tsotsi-style storytelling, motivational writing, and engaging
        social media content. My goal is to grow into a powerful screen actor and influential creative.
      </p>
    </div>

    <div className="bg-zinc-900 rounded-3xl p-8 border border-zinc-800 shadow-2xl">
      <h3 className="text-2xl font-bold mb-6">Quick Info</h3>

      <div className="space-y-4 text-zinc-300">
        <div className="flex justify-between border-b border-zinc-800 pb-3">
          <span>Phone</span>
          <span>067 569 4562</span>
        </div>

        <div className="flex justify-between border-b border-zinc-800 pb-3">
          <span>Email</span>
          <span className="text-right">thabomasilela2804@gmail.com</span>
        </div>
        <div className="flex justify-between border-b border-zinc-800 pb-3">
          <span>Age</span>
          <span>18 Years Old</span>
        </div>

        <div className="flex justify-between border-b border-zinc-800 pb-3">
          <span>Location</span>
          <span>Johannesburg, South Africa</span>
        </div>

        <div className="flex justify-between border-b border-zinc-800 pb-3">
          <span>Industry</span>
          <span>Film & Digital Media</span>
        </div>

        <div className="flex justify-between">
          <span>Current Role</span>
          <span>Court 4 — Native Eye Creative SA</span>
        </div>
      </div>
    </div>
  </section>

  {/* Skills */}
  <section className="px-6 py-10 bg-black">
    <div className="max-w-6xl mx-auto grid md:grid-cols-4 gap-6">
      {[
        ['Projects', '10+'],
        ['Creative Roles', 'Actor'],
        ['Content Style', 'Motivational'],
        ['Location', 'South Africa'],
      ].map((item, index) => (
        <div
          key={index}
          className="bg-zinc-900 border border-zinc-800 rounded-3xl p-6 text-center shadow-xl"
        >
          <h3 className="text-3xl font-extrabold text-red-500 mb-2">{item[1]}</h3>
          <p className="text-zinc-400 tracking-wide uppercase text-sm">{item[0]}</p>
        </div>
      ))}
    </div>
  </section>

  <section className="bg-zinc-950 px-6 py-20">
    <div className="max-w-6xl mx-auto">
      <h2 className="text-4xl md:text-5xl font-bold text-center mb-4">Skills & Expertise</h2>

      <p className="text-zinc-400 text-center max-w-2xl mx-auto mb-14 leading-7">
        Combining acting performance, street-inspired storytelling, and digital creativity to create impactful entertainment experiences.
      </p>

      <div className="grid md:grid-cols-3 gap-8">
        {[
          {
            title: 'Acting',
            desc: 'Dramatic scenes, emotional storytelling, character interpretation, and performance delivery.',
          },
          {
            title: 'Content Creation',
            desc: 'Creative short-form videos, motivational content, and social media engagement.',
          },
          {
            title: 'Script Writing',
            desc: 'Tsotsi-style storytelling, dialogue writing, and original entertainment concepts.',
          },
        ].map((item, index) => (
          <div
            key={index}
            className="bg-black border border-zinc-800 rounded-3xl p-8 hover:border-red-500 transition"
          >
            <h3 className="text-2xl font-bold mb-4">{item.title}</h3>
            <p className="text-zinc-400 leading-7">{item.desc}</p>
          </div>
        ))}
      </div>
    </div>
  </section>

  {/* Projects */}
  <section id="work" className="px-6 py-28 max-w-7xl mx-auto">
    <div className="flex items-end justify-between mb-16 flex-wrap gap-6">
      <div>
        <p className="uppercase tracking-[0.3em] text-red-400 text-sm mb-4">
          Selected Work
        </p>

        <h2 className="text-5xl md:text-6xl font-black leading-tight">
          Creative
          <br />
          Portfolio
        </h2>
      </div>

      <p className="text-zinc-400 max-w-md leading-8 text-lg">
        A growing collection of acting performances, digital storytelling projects, and creative concepts.
      </p>
    </div>

    <div className="grid lg:grid-cols-3 gap-8">
      {featuredProjects.map((project, index) => (
        <div
          key={index}
          className="group bg-gradient-to-b from-zinc-900 to-black border border-zinc-800 rounded-[32px] p-8 shadow-2xl hover:border-red-500/40 transition duration-300 hover:-translate-y-2"
        >
          <div className="flex items-center justify-between mb-5">
            <p className="text-red-400 uppercase tracking-widest text-sm">
              {project.type}
          </p>

          <h3 className="text-2xl font-bold mb-4">{project.title}</h3>

          <p className="text-zinc-400 leading-7">{project.desc}</p>
        </div>
      ))}
    </div>
  </section>

  {/* Contact */}
  <section id="contact" className="bg-gradient-to-t from-zinc-900 to-black px-6 py-24">
    <div className="max-w-6xl mx-auto grid lg:grid-cols-2 gap-16 items-center">
      <div>
        <p className="uppercase tracking-[0.3em] text-red-400 text-sm mb-4">
          Contact & Bookings
        </p>

        <h2 className="text-5xl font-black mb-6 leading-tight">
          Let’s Create
          <br />
          Something Powerful
        </h2>

        <p className="text-zinc-400 text-lg leading-8 mb-10">
          Available for acting opportunities, creative collaborations, interviews, campaigns, and digital partnerships.
        </p>

        <div className="space-y-5 text-lg">
          <p>
            <span className="text-zinc-500">Email:</span> thabomasilela2804@gmail.com
          </p>

          <p>
            <span className="text-zinc-500">Phone:</span> 067 569 4562
          </p>

          <p>
            <span className="text-zinc-500">Location:</span> Johannesburg, South Africa
          </p>
        </div>
      </div>

      <div className="bg-black border border-zinc-800 rounded-[32px] p-8 shadow-2xl">
        <form className="space-y-6">
          <input
            type="text"
            placeholder="Your Name"
            className="w-full bg-zinc-900 border border-zinc-800 rounded-2xl px-5 py-4 outline-none focus:border-red-500"
          />

          <input
            type="email"
            placeholder="Your Email"
            className="w-full bg-zinc-900 border border-zinc-800 rounded-2xl px-5 py-4 outline-none focus:border-red-500"
          />

          <textarea
            rows="5"
            placeholder="Tell me about your project..."
            className="w-full bg-zinc-900 border border-zinc-800 rounded-2xl px-5 py-4 outline-none focus:border-red-500"
          />

          <button
            type="submit"
            className="w-full bg-red-600 hover:bg-red-700 transition py-4 rounded-2xl font-bold text-lg"
          >
            Send Message
          </button>
        </form>
      </div>
    </div>

    <div className="max-w-3xl mx-auto text-center mt-24">
    <div className="max-w-3xl mx-auto">
      <h2 className="text-5xl font-bold mb-6">Let’s Work Together</h2>

      <p className="text-zinc-400 text-lg leading-8 mb-10">
        Open to acting opportunities, collaborations, content partnerships, and creative projects.
      </p>

      <div className="flex flex-wrap justify-center gap-4">
        <a
          href="mailto:thabomasilela2804@gmail.com"
          className="bg-white text-black font-bold px-8 py-4 rounded-2xl hover:scale-105 transition inline-block"
        >
          Email Me
        </a>

        <a
          href="https://www.instagram.com/thabo_msikelave?igsh=MTZkYTloOGR5cmswNw="
          target="_blank"
          rel="noopener noreferrer"
          className="border border-white px-8 py-4 rounded-2xl hover:bg-white hover:text-black transition inline-block"
        >
          Instagram
        </a>

        <a
          href="https://tiktok.com/@msekelave_"
          target="_blank"
          rel="noopener noreferrer"
          className="border border-red-500 text-red-400 px-8 py-4 rounded-2xl hover:bg-red-500 hover:text-white transition inline-block"
        >
          TikTok
        </a>
      </div>
    </div>
  </section>

  {/* Footer */}
  <section className="px-6 py-20 bg-zinc-950">
    <div className="max-w-4xl mx-auto text-center">
      <h2 className="text-4xl font-bold mb-6">Follow My Journey</h2>

      <p className="text-zinc-400 leading-8 mb-10 text-lg">
        Follow me on social media for acting updates, motivational content, behind-the-scenes moments, and creative storytelling.
      </p>

      <div className="grid md:grid-cols-2 gap-8 mb-14">
        <div className="bg-black border border-zinc-800 rounded-[28px] overflow-hidden shadow-2xl">
          <img
            src="/mnt/data/Screenshot_2026-05-24-15-54-12-872_com.instagram.android.jpg"
            alt="Instagram Profile"
            className="w-full h-full object-cover"
          />
        </div>

        <div className="bg-black border border-zinc-800 rounded-[28px] overflow-hidden shadow-2xl">
          <img
            src="/mnt/data/Screenshot_2026-05-24-15-50-16-944_com.zhiliaoapp.musically.jpg"
            alt="TikTok Profile"
            className="w-full h-full object-cover"
          />
        </div>
      </div>

      <div className="flex flex-wrap justify-center gap-6 text-lg">
        <a
          href="https://www.instagram.com/thabo_msikelave?igsh=MTZkYTloOGR5cmswNw="
          target="_blank"
          rel="noopener noreferrer"
          className="bg-gradient-to-r from-pink-500 to-red-500 px-8 py-4 rounded-2xl font-bold hover:scale-105 transition"
        >
          Instagram
        </a>

        <a
          href="https://tiktok.com/@msekelave_"
          target="_blank"
          rel="noopener noreferrer"
          className="bg-white text-black px-8 py-4 rounded-2xl font-bold hover:scale-105 transition"
        >
          TikTok
        </a>
      </div>
    </div>
  </section>

  <footer className="border-t border-zinc-900 py-8 text-center text-zinc-500 text-sm">
    © 2026 Thabo Masilela. All Rights Reserved.
  </footer>
</div>

) }export default function ThaboPortfolio() { const featuredProjects = [ { title: 'Court 4 — Native Eye Creative SA', type: 'Lead Performance', year: '2026', description: 'A dramatic acting role focused on authentic township storytelling and emotional realism.', }, { title: 'Motivational Digital Content', type: 'Creator Brand', year: '2026', description: 'Short-form inspirational content designed to motivate and connect with young audiences.', }, { title: 'Street Storytelling Concepts', type: 'Creative Writing', year: '2025', description: 'Original scripts inspired by tsotsi-style storytelling, youth culture, and township experiences.', }, ]

return ( <div className="min-h-screen bg-black text-white font-sans overflow-hidden"> {{/* Navigation */} <nav className="fixed top-0 left-0 right-0 z-50 backdrop-blur-xl bg-black/70 border-b border-zinc-900"> <div className="max-w-7xl mx-auto px-6 py-5 flex items-center justify-between"> <h1 className="text-2xl font-black tracking-widest"> THABO<span className="text-red-500">.</span> </h1>

<div className="hidden md:flex items-center gap-8 text-sm uppercase tracking-wider text-zinc-400">
        <a href="#about" className="hover:text-white transition">About</a>
        <a href="#work" className="hover:text-white transition">Portfolio</a>
        <a href="#contact" className="hover:text-white transition">Contact</a>
      </div>
    </div>
  </nav>

  {/* Hero Section */}
  <section className="relative min-h-screen flex items-center px-6 overflow-hidden">
    <div className="absolute inset-0 bg-gradient-to-br from-red-950/20 via-black to-black" />

    <div className="absolute top-20 right-10 w-72 h-72 bg-red-600/20 rounded-full blur-3xl" />
    <div className="absolute bottom-10 left-10 w-72 h-72 bg-zinc-700/20 rounded-full blur-3xl" />

    <div className="relative z-10 max-w-7xl mx-auto grid lg:grid-cols-2 gap-16 items-center w-full pt-24">
      <div>
        <p className="uppercase tracking-[0.4em] text-red-400 mb-6 text-sm font-semibold">
          South African Actor & Creative
        </p>

        <h1 className="text-6xl md:text-8xl font-black leading-none mb-8">
          THABO
          <br />
          <span className="text-zinc-500">MASILELA</span>
        </h1>

        <p className="text-xl text-zinc-300 leading-9 mb-10 max-w-2xl">
          Building a bold creative identity through acting, storytelling, and youth-driven digital content.
          Focused on cinematic performances, authentic expression, and impactful entertainment.
        </p>

        <div className="flex flex-wrap gap-5">
          <a
            href="#work"
            className="bg-red-600 hover:bg-red-700 transition px-8 py-4 rounded-2xl font-bold shadow-2xl"
          >
            View Portfolio
          </a>

          <a
            href="#contact"
            className="border border-zinc-700 hover:border-white transition px-8 py-4 rounded-2xl font-bold"
          >
            Contact Me
          </a>
        </div>
      </div>

      <div className="relative">
        <div className="bg-gradient-to-b from-zinc-900 to-black border border-zinc-800 rounded-[40px] p-10 shadow-2xl">
          <div className="aspect-[4/5] rounded-[30px] bg-zinc-950 border border-zinc-800 flex items-center justify-center text-center p-6 overflow-hidden">
            <img
              src="/mnt/data/file_00000000e1fc722f9fa7c9e946dc42fc.jpg"
              alt="Thabo Masilela"
              className="w-full h-full object-cover rounded-[24px]"
            />
            <div>
              <p className="text-red-400 uppercase tracking-[0.3em] text-sm mb-6 font-semibold">
                Official Creative Portfolio
              </p>

              <h2 className="text-5xl font-black leading-tight mb-4">
                Actor.
                <br />
                Creator.
                <br />
                Storyteller.
              </h2>

              <p className="text-zinc-400 leading-8 text-lg">
                Johannesburg-based upcoming actor creating modern African entertainment experiences.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  {/* About */}}
  <section id="about" className="px-6 py-28 max-w-7xl mx-auto grid lg:grid-cols-2 gap-16 items-center">
    <div>
      <h2 className="text-4xl font-bold mb-6">About Me</h2>

      <p className="text-zinc-300 leading-8 text-lg mb-5">
        I am a young creative from South Africa building my journey in the entertainment industry.
        My work focuses on acting, storytelling, digital content, and inspiring young people through
        authentic and relatable experiences.
      </p>

      <p className="text-zinc-400 leading-8">
        I enjoy dramatic performances, tsotsi-style storytelling, motivational writing, and engaging
        social media content. My goal is to grow into a powerful screen actor and influential creative.
      </p>
    </div>

    <div className="bg-zinc-900 rounded-3xl p-8 border border-zinc-800 shadow-2xl">
      <h3 className="text-2xl font-bold mb-6">Quick Info</h3>

      <div className="space-y-4 text-zinc-300">
        <div className="flex justify-between border-b border-zinc-800 pb-3">
          <span>Phone</span>
          <span>067 569 4562</span>
        </div>

        <div className="flex justify-between border-b border-zinc-800 pb-3">
          <span>Email</span>
          <span className="text-right">thabomasilela2804@gmail.com</span>
        </div>
        <div className="flex justify-between border-b border-zinc-800 pb-3">
          <span>Age</span>
          <span>18 Years Old</span>
        </div>

        <div className="flex justify-between border-b border-zinc-800 pb-3">
          <span>Location</span>
          <span>Johannesburg, South Africa</span>
        </div>

        <div className="flex justify-between border-b border-zinc-800 pb-3">
          <span>Industry</span>
          <span>Film & Digital Media</span>
        </div>

        <div className="flex justify-between">
          <span>Current Role</span>
          <span>Court 4 — Native Eye Creative SA</span>
        </div>
      </div>
    </div>
  </section>

  {/* Skills */}
  <section className="px-6 py-10 bg-black">
    <div className="max-w-6xl mx-auto grid md:grid-cols-4 gap-6">
      {[
        ['Projects', '10+'],
        ['Creative Roles', 'Actor'],
        ['Content Style', 'Motivational'],
        ['Location', 'South Africa'],
      ].map((item, index) => (
        <div
          key={index}
          className="bg-zinc-900 border border-zinc-800 rounded-3xl p-6 text-center shadow-xl"
        >
          <h3 className="text-3xl font-extrabold text-red-500 mb-2">{item[1]}</h3>
          <p className="text-zinc-400 tracking-wide uppercase text-sm">{item[0]}</p>
        </div>
      ))}
    </div>
  </section>

  <section className="bg-zinc-950 px-6 py-20">
    <div className="max-w-6xl mx-auto">
      <h2 className="text-4xl md:text-5xl font-bold text-center mb-4">Skills & Expertise</h2>

      <p className="text-zinc-400 text-center max-w-2xl mx-auto mb-14 leading-7">
        Combining acting performance, street-inspired storytelling, and digital creativity to create impactful entertainment experiences.
      </p>

      <div className="grid md:grid-cols-3 gap-8">
        {[
          {
            title: 'Acting',
            desc: 'Dramatic scenes, emotional storytelling, character interpretation, and performance delivery.',
          },
          {
            title: 'Content Creation',
            desc: 'Creative short-form videos, motivational content, and social media engagement.',
          },
          {
            title: 'Script Writing',
            desc: 'Tsotsi-style storytelling, dialogue writing, and original entertainment concepts.',
          },
        ].map((item, index) => (
          <div
            key={index}
            className="bg-black border border-zinc-800 rounded-3xl p-8 hover:border-red-500 transition"
          >
            <h3 className="text-2xl font-bold mb-4">{item.title}</h3>
            <p className="text-zinc-400 leading-7">{item.desc}</p>
          </div>
        ))}
      </div>
    </div>
  </section>

  {/* Projects */}
  <section id="work" className="px-6 py-28 max-w-7xl mx-auto">
    <div className="flex items-end justify-between mb-16 flex-wrap gap-6">
      <div>
        <p className="uppercase tracking-[0.3em] text-red-400 text-sm mb-4">
          Selected Work
        </p>

        <h2 className="text-5xl md:text-6xl font-black leading-tight">
          Creative
          <br />
          Portfolio
        </h2>
      </div>

      <p className="text-zinc-400 max-w-md leading-8 text-lg">
        A growing collection of acting performances, digital storytelling projects, and creative concepts.
      </p>
    </div>

    <div className="grid lg:grid-cols-3 gap-8">
      {featuredProjects.map((project, index) => (
        <div
          key={index}
          className="group bg-gradient-to-b from-zinc-900 to-black border border-zinc-800 rounded-[32px] p-8 shadow-2xl hover:border-red-500/40 transition duration-300 hover:-translate-y-2"
        >
          <div className="flex items-center justify-between mb-5">
            <p className="text-red-400 uppercase tracking-widest text-sm">
              {project.type}
          </p>

          <h3 className="text-2xl font-bold mb-4">{project.title}</h3>

          <p className="text-zinc-400 leading-7">{project.desc}</p>
        </div>
      ))}
    </div>
  </section>

  {/* Contact */}
  <section id="contact" className="bg-gradient-to-t from-zinc-900 to-black px-6 py-24">
    <div className="max-w-6xl mx-auto grid lg:grid-cols-2 gap-16 items-center">
      <div>
        <p className="uppercase tracking-[0.3em] text-red-400 text-sm mb-4">
          Contact & Bookings
        </p>

        <h2 className="text-5xl font-black mb-6 leading-tight">
          Let’s Create
          <br />
          Something Powerful
        </h2>

        <p className="text-zinc-400 text-lg leading-8 mb-10">
          Available for acting opportunities, creative collaborations, interviews, campaigns, and digital partnerships.
        </p>

        <div className="space-y-5 text-lg">
          <p>
            <span className="text-zinc-500">Email:</span> thabomasilela2804@gmail.com
          </p>

          <p>
            <span className="text-zinc-500">Phone:</span> 067 569 4562
          </p>

          <p>
            <span className="text-zinc-500">Location:</span> Johannesburg, South Africa
          </p>
        </div>
      </div>

      <div className="bg-black border border-zinc-800 rounded-[32px] p-8 shadow-2xl">
        <form className="space-y-6">
          <input
            type="text"
            placeholder="Your Name"
            className="w-full bg-zinc-900 border border-zinc-800 rounded-2xl px-5 py-4 outline-none focus:border-red-500"
          />

          <input
            type="email"
            placeholder="Your Email"
            className="w-full bg-zinc-900 border border-zinc-800 rounded-2xl px-5 py-4 outline-none focus:border-red-500"
          />

          <textarea
            rows="5"
            placeholder="Tell me about your project..."
            className="w-full bg-zinc-900 border border-zinc-800 rounded-2xl px-5 py-4 outline-none focus:border-red-500"
          />

          <button
            type="submit"
            className="w-full bg-red-600 hover:bg-red-700 transition py-4 rounded-2xl font-bold text-lg"
          >
            Send Message
          </button>
        </form>
      </div>
    </div>

    <div className="max-w-3xl mx-auto text-center mt-24">
    <div className="max-w-3xl mx-auto">
      <h2 className="text-5xl font-bold mb-6">Let’s Work Together</h2>

      <p className="text-zinc-400 text-lg leading-8 mb-10">
        Open to acting opportunities, collaborations, content partnerships, and creative projects.
      </p>

      <div className="flex flex-wrap justify-center gap-4">
        <a
          href="mailto:thabomasilela2804@gmail.com"
          className="bg-white text-black font-bold px-8 py-4 rounded-2xl hover:scale-105 transition inline-block"
        >
          Email Me
        </a>

        <a
          href="https://www.instagram.com/thabo_msikelave?igsh=MTZkYTloOGR5cmswNw="
          target="_blank"
          rel="noopener noreferrer"
          className="border border-white px-8 py-4 rounded-2xl hover:bg-white hover:text-black transition inline-block"
        >
          Instagram
        </a>

        <a
          href="https://tiktok.com/@msekelave_"
          target="_blank"
          rel="noopener noreferrer"
          className="border border-red-500 text-red-400 px-8 py-4 rounded-2xl hover:bg-red-500 hover:text-white transition inline-block"
        >
          TikTok
        </a>
      </div>
    </div>
  </section>

  {/* Footer */}
  <section className="px-6 py-20 bg-zinc-950">
    <div className="max-w-4xl mx-auto text-center">
      <h2 className="text-4xl font-bold mb-6">Follow My Journey</h2>

      <p className="text-zinc-400 leading-8 mb-10 text-lg">
        Follow me on social media for acting updates, motivational content, behind-the-scenes moments, and creative storytelling.
      </p>

      <div className="grid md:grid-cols-2 gap-8 mb-14">
        <div className="bg-black border border-zinc-800 rounded-[28px] overflow-hidden shadow-2xl">
          <img
            src="/mnt/data/Screenshot_2026-05-24-15-54-12-872_com.instagram.android.jpg"
            alt="Instagram Profile"
            className="w-full h-full object-cover"
          />
        </div>

        <div className="bg-black border border-zinc-800 rounded-[28px] overflow-hidden shadow-2xl">
          <img
            src="/mnt/data/Screenshot_2026-05-24-15-50-16-944_com.zhiliaoapp.musically.jpg"
            alt="TikTok Profile"
            className="w-full h-full object-cover"
          />
        </div>
      </div>

      <div className="flex flex-wrap justify-center gap-6 text-lg">
        <a
          href="https://www.instagram.com/thabo_msikelave?igsh=MTZkYTloOGR5cmswNw="
          target="_blank"
          rel="noopener noreferrer"
          className="bg-gradient-to-r from-pink-500 to-red-500 px-8 py-4 rounded-2xl font-bold hover:scale-105 transition"
        >
          Instagram
        </a>

        <a
          href="https://tiktok.com/@msekelave_"
          target="_blank"
          rel="noopener noreferrer"
          className="bg-white text-black px-8 py-4 rounded-2xl font-bold hover:scale-105 transition"
        >
          TikTok
        </a>
      </div>
    </div>
  </section>

  <footer className="border-t border-zinc-900 py-8 text-center text-zinc-500 text-sm">
    © 2026 Thabo Masilela. All Rights Reserved.
  </footer>
</div>

) }
