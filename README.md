# rutvik-ielts-website
Official website for Rutvik IELTS YouTube channel
import React from "react"; import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { Youtube } from "lucide-react"; import { motion } from "framer-motion";

export default function RutvikIELTS() { return ( <div className="min-h-screen bg-white text-gray-800 p-6 md:p-12"> <motion.header initial={{ opacity: 0, y: -30 }} animate={{ opacity: 1, y: 0 }} transition={{ duration: 0.8 }} className="text-center mb-10" > <h1 className="text-4xl md:text-6xl font-bold text-blue-700 mb-4"> Rutvik IELTS </h1> <p className="text-lg md:text-2xl text-gray-600"> Your Gateway to IELTS Success – Tips, Practice, and Strategy Videos </p> </motion.header>

<div className="grid grid-cols-1 md:grid-cols-3 gap-6">
    <Card className="rounded-2xl shadow-xl hover:shadow-2xl transition-all">
      <CardContent className="p-6">
        <h2 className="text-xl font-semibold mb-2">🎯 IELTS Strategy Videos</h2>
        <p className="text-sm text-gray-600">
          Learn smart tips and proven strategies to crack Listening, Reading, Writing & Speaking.
        </p>
      </CardContent>
    </Card>

    <Card className="rounded-2xl shadow-xl hover:shadow-2xl transition-all">
      <CardContent className="p-6">
        <h2 className="text-xl font-semibold mb-2">🎧 Listening Practice</h2>
        <p className="text-sm text-gray-600">
          Improve your band score with real test-style listening materials and questions.
        </p>
      </CardContent>
    </Card>

    <Card className="rounded-2xl shadow-xl hover:shadow-2xl transition-all">
      <CardContent className="p-6">
        <h2 className="text-xl font-semibold mb-2">📚 Free Resources</h2>
        <p className="text-sm text-gray-600">
          Access PDF books and join our Telegram for exclusive practice content.
        </p>
      </CardContent>
    </Card>
  </div>

  <motion.div
    initial={{ opacity: 0, y: 30 }}
    animate={{ opacity: 1, y: 0 }}
    transition={{ delay: 0.5, duration: 0.8 }}
    className="mt-12 text-center"
  >
    <Button asChild className="text-lg px-8 py-4 rounded-2xl">
      <a
        href="https://youtube.com/@rutvikielts263"
        target="_blank"
        rel="noopener noreferrer"
        className="flex items-center gap-2"
      >
        <Youtube className="w-6 h-6" />
        Visit My YouTube Channel
      </a>
    </Button>
  </motion.div>
</div>

); }

