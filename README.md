# My-gedo


import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { motion } from "framer-motion";

const HomePage = () => {
  return (
    <div className="bg-black text-white min-h-screen">
      {/* Header */}
      <header className="flex justify-between items-center p-6 border-b border-gray-800">
        <h1 className="text-3xl font-bold">MyStore</h1>
        <nav>
          <ul className="flex gap-6">
            <li><a href="#" className="hover:text-gray-400">رجالي</a></li>
            <li><a href="#" className="hover:text-gray-400">نساء</a></li>
          </ul>
        </nav>
      </header>
      
      {/* Hero Section */}
      <section className="text-center py-20">
        <h2 className="text-5xl font-extrabold">اكتشف الأناقة</h2>
        <p className="text-gray-400 mt-4">أحدث صيحات الموضة بجودة فاخرة</p>
        <Button className="mt-6 bg-white text-black px-6 py-2 rounded-full hover:bg-gray-200">تسوق الآن</Button>
      </section>
      
      {/* Featured Products */}
      <section className="grid grid-cols-2 md:grid-cols-4 gap-6 p-6">
        {[1, 2, 3, 4].map((item) => (
          <motion.div key={item} whileHover={{ scale: 1.05 }}>
            <Card className="bg-gray-900 rounded-lg overflow-hidden">
              <CardContent>
                <img src="https://via.placeholder.com/300" alt="Product" className="w-full" />
                <h3 className="text-lg mt-2">منتج فاخر</h3>
                <p className="text-gray-400">$99.99</p>
              </CardContent>
            </Card>
          </motion.div>
        ))}
      </section>
    </div>
  );
};

export default HomePage;
