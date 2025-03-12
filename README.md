import { motion } from "framer-motion";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

export default function HomePage() {
  return (
    <div className="bg-black text-white min-h-screen">
      {/* Hero Section */}
      <section className="text-center py-20">
        <h2 className="text-5xl font-extrabold">اكتشف الأناقة</h2>
        <p className="text-gray-400 mt-4">أحدث صيحات الموضة بجودة فاخرة</p>
        <Button className="mt-6 bg-white text-black px-6 py-2 rounded-full hover:bg-gray-200">
          تسوق الآن
        </Button>
      </section>

      {/* Featured Products */}
      <section className="grid grid-cols-2 md:grid-cols-4 gap-6 p-6">
        {[1, 2, 3, 4].map((item) => (
          <motion.div key={item} whileHover={{ scale: 1.05 }}>
            <Card className="bg-gray-900 rounded-lg overflow-hidden">
              <CardContent>
                <img src={`/images/product-${item}.jpg`} alt="منتج فاخر" className="w-full rounded-t-lg" />
                <h3 className="text-lg mt-2 font-semibold">منتج فاخر</h3>
                <p className="text-gray-400">$99.99</p>
              </CardContent>
            </Card>
          </motion.div>
        ))}
      </section>
    </div>
  );
}
