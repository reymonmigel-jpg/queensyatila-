import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { Heart, Calendar, Image, Phone } from "lucide-react"; import { motion } from "framer-motion";

export default function WeddingOrganizerWebsite() { return ( <div className="min-h-screen bg-[#0f0f0f] text-white font-serif"> {/* Hero Section */} <section className="relative h-screen flex items-center justify-center text-center px-6"> <motion.div initial={{ opacity: 0, y: 30 }} animate={{ opacity: 1, y: 0 }} transition={{ duration: 1 }} > <h1 className="text-4xl md:text-6xl font-bold tracking-wide text-gold"> Elegant Wedding Organizer </h1> <p className="mt-4 text-lg md:text-xl text-gray-300"> Mewujudkan Pernikahan Impian dengan Sentuhan Elegan & Berkelas </p> <Button className="mt-8 bg-gold text-black hover:opacity-80 rounded-2xl px-8 py-6"> Konsultasi Sekarang </Button> </motion.div> </section>

{/* About Section */}
  <section className="py-20 px-6 md:px-20 bg-[#141414]">
    <motion.div initial={{ opacity: 0 }} whileInView={{ opacity: 1 }} transition={{ duration: 1 }}>
      <h2 className="text-3xl md:text-4xl mb-6 text-gold">Tentang Kami</h2>
      <p className="text-gray-300 max-w-3xl">
        Kami adalah Wedding Organizer profesional yang berfokus pada konsep elegan,
        intimate, dan luxury wedding. Dengan pengalaman dan tim terbaik, kami siap
        mendampingi setiap momen sakral Anda agar berjalan sempurna.
      </p>
    </motion.div>
  </section>

  {/* Services */}
  <section className="py-20 px-6 md:px-20">
    <h2 className="text-3xl md:text-4xl mb-12 text-center text-gold">Layanan Kami</h2>
    <div className="grid md:grid-cols-3 gap-8">
      {[{ icon: Heart, title: "Full Wedding Planning" }, { icon:
