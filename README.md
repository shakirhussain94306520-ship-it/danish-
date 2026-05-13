export default function SKDeresWebsite() {
  return (
    <div className="min-h-screen bg-white text-black">
      {/* Navbar */}
      <header className="flex items-center justify-between px-8 py-5 border-b sticky top-0 bg-white/90 backdrop-blur z-10">
        <h1 className="text-2xl font-bold tracking-[0.25em]">SK DERES</h1>
        <nav className="hidden md:flex gap-8 text-sm uppercase tracking-wide">
          <a href="#home" className="hover:opacity-70">Home</a>
          <a href="#collection" className="hover:opacity-70">Collection</a>
          <a href="#about" className="hover:opacity-70">About</a>
          <a href="#contact" className="hover:opacity-70">Contact</a>
        </nav>
      </header>

      {/* Hero */}
      <section id="home" className="grid md:grid-cols-2 items-center px-8 md:px-16 py-20 gap-10">
        <div>
          <p className="uppercase text-sm tracking-[0.3em] text-gray-500 mb-4">
            Modern Minimal Clothing
          </p>
          <h2 className="text-5xl md:text-7xl font-bold leading-tight">
            Wear Your Style.
          </h2>
          <p className="mt-6 text-gray-600 text-lg max-w-lg">
            SK Deres brings modern minimal fashion with premium comfort and clean style.
          </p>
          <button className="mt-8 bg-black text-white px-8 py-3 rounded-2xl hover:opacity-90 transition">
            Shop Now
          </button>
        </div>

        <div>
          <img
            src="https://images.unsplash.com/photo-1523398002811-999ca8dec234?q=80&w=1200&auto=format&fit=crop"
            alt="Fashion"
            className="rounded-[2rem] shadow-xl w-full h-[500px] object-cover"
          />
        </div>
      </section>

      {/* Collection */}
      <section id="collection" className="px-8 md:px-16 py-20 bg-gray-50">
        <h3 className="text-4xl font-bold mb-10">Featured Collection</h3>
        <div className="grid md:grid-cols-3 gap-6">
          {[
            'Oversized T-Shirts',
            'Minimal Hoodies',
            'Street Jackets'
          ].map((item) => (
            <div key={item} className="bg-white rounded-[2rem] overflow-hidden shadow-sm hover:shadow-lg transition p-5">
              <div className="bg-gray-200 h-72 rounded-2xl mb-4" />
              <h4 className="text-xl font-semibold">{item}</h4>
              <p className="text-gray-500 mt-2">Premium comfort and clean minimal design.</p>
            </div>
          ))}
        </div>
      </section>

      {/* About */}
      <section id="about" className="px-8 md:px-16 py-20 text-center max-w-4xl mx-auto">
        <h3 className="text-4xl font-bold mb-6">About SK Deres</h3>
        <p className="text-gray-600 text-lg leading-8">
          SK Deres is a modern minimal clothing brand focused on simple, stylish, and comfortable fashion for everyday wear.
        </p>
      </section>

      {/* Contact */}
      <section id="contact" className="px-8 md:px-16 py-20 bg-black text-white text-center rounded-t-[3rem]">
        <h3 className="text-4xl font-bold">Contact Us</h3>
        <p className="text-gray-300 mt-4">Instagram: @skderes</p>
        <p className="text-gray-300">Email: contact@skderes.com</p>
      </section>
    </div>
  );
}
