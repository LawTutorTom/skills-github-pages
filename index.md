---
import { Card, CardContent } from "@/components/ui/card";
import { Mail, Phone } from "lucide-react";
import { motion } from "framer-motion";

export default function BarExamTutorLandingPage() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-white to-blue-50 text-gray-900">
      <header className="p-6 text-center shadow-sm bg-white">
        <h1 className="text-4xl font-bold">Bar Exam Mastery</h1>
        <p className="text-lg mt-2">One-on-one tutoring to help you pass with confidence</p>
      </header>

      <main className="flex flex-col lg:flex-row gap-8 p-6 max-w-5xl mx-auto">
        <motion.section 
          initial={{ opacity: 0, y: 30 }} 
          animate={{ opacity: 1, y: 0 }} 
          transition={{ duration: 0.6 }}
          className="flex-1 space-y-6"
        >
          <h2 className="text-2xl font-semibold">Why Choose Me?</h2>
          <ul className="list-disc list-inside space-y-2">
            <li>Former bar exam grader and licensed attorney</li>
            <li>Tailored study plans for your learning style</li>
            <li>Flexible scheduling with Zoom or in-person sessions</li>
            <li>Extensive MBE and essay preparation strategies</li>
          </ul>

          <Card className="bg-white shadow-md">
            <CardContent className="p-6 text-sm text-gray-700 space-y-2">
              <h3 className="text-lg font-medium">Contact Information</h3>
              <p className="flex items-center gap-2"><Mail size={16} /> tutor@example.com</p>
              <p className="flex items-center gap-2"><Phone size={16} /> (123) 456-7890</p>
            </CardContent>
          </Card>
        </motion.section>

        <motion.section 
          initial={{ opacity: 0, y: 30 }} 
          animate={{ opacity: 1, y: 0 }} 
          transition={{ duration: 0.6, delay: 0.2 }}
          className="flex-1"
        >
          <img 
            src="https://images.unsplash.com/photo-1581092160613-eb7f28c7b1ef?fit=crop&w=800&q=80" 
            alt="Studying for bar exam" 
            className="w-full rounded-2xl shadow-lg"
          />
        </motion.section>
      </main>

      <footer className="text-center p-4 text-sm text-gray-500 bg-white border-t">
        &copy; {new Date().getFullYear()} Bar Exam Mastery. All rights reserved.
      </footer>
    </div>
  );
}

---
