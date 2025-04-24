import React from "react";
import { Button } from "@/components/ui/button";
import { Phone, Mail, Car, Key, Clock, MapPin, CheckCircle, MessageCircle, KeyRound } from "lucide-react";
import { Badge } from "@/components/ui/badge";

export default function Landing() {
  const whatsappLink = "https://wa.me/972555576780?text=" + encodeURIComponent("שלום בנימין, ראיתי את האתר שלך ואני זקוק לשירותי מנעולן רכב. אפשר פרטים?");
  
  return (
    <div className="min-h-screen bg-gradient-to-b from-blue-50 to-white" dir="rtl">
      {/* Hero Section */}
      <div className="bg-blue-600 text-white">
        <div className="max-w-6xl mx-auto px-4 py-16 md:py-24">
          <div className="text-center relative">
            <div className="absolute top-0 left-1/2 transform -translate-x-1/2 -translate-y-1/2">
              <Badge className="bg-red-500 text-white animate-pulse">
                <Clock className="w-4 h-4 mr-1" />
                שירות 24/7
              </Badge>
            </div>
            <img 
              src="https://qtrypzzcjebvfcihiynt.supabase.co/storage/v1/object/public/base44-prod/public/594d78_IMG-20250413-WA0027.jpg"
              alt="בנימין מנעולן רכב"
              className="w-48 h-48 mx-auto mb-8 rounded-full shadow-lg"
            />
            <h1 className="text-4xl md:text-6xl font-bold mb-6">בנימין מנעולן רכב</h1>
            <p className="text-xl md:text-2xl mb-8">פתרונות מנעול מקצועיים לרכב שלך 24/7</p>
            <div className="flex flex-col md:flex-row gap-4 justify-center items-center">
              <Button 
                size="lg"
                className="bg-white text-blue-600 hover:bg-blue-50 text-lg gap-2 transform transition-transform hover:scale-105"
                onClick={() => window.location.href = 'tel:972555576780'}
              >
                <Phone className="w-5 h-5" />
                055-557-6780
              </Button>
              <Button 
                size="lg"
                className="bg-green-500 hover:bg-green-600 text-white text-lg gap-2 transform transition-transform hover:scale-105"
                onClick={() => window.location.href = whatsappLink}
              >
                <MessageCircle className="w-5 h-5" />
                WhatsApp
              </Button>
            </div>
          </div>
        </div>
      </div>

      {/* Services */}
      <div className="max-w-6xl mx-auto px-4 py-16">
        <h2 className="text-3xl font-bold text-center mb-12">השירותים שלנו</h2>
        <div className="grid md:grid-cols-3 gap-8">
          <div className="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition-shadow">
            <Car className="w-12 h-12 text-blue-600 mb-4" />
            <h3 className="text-xl font-bold mb-2">פתיחת רכבים</h3>
            <p className="text-gray-600">פתיחה מקצועית של כל סוגי הרכבים ללא נזק</p>
          </div>
          <div className="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition-shadow">
            <Key className="w-12 h-12 text-blue-600 mb-4" />
            <h3 className="text-xl font-bold mb-2">שחזור ושכפול מפתחות</h3>
            <p className="text-gray-600">שחזור ושכפול מפתחות לכל סוגי הרכבים</p>
          </div>
          <div className="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition-shadow">
            <KeyRound className="w-12 h-12 text-blue-600 mb-4" />
            <h3 className="text-xl font-bold mb-2">תיקון סוויץ'</h3>
            <p className="text-gray-600">תיקון מקצועי של מנעול ההתנעה ברכב</p>
          </div>
        </div>
      </div>

      {/* Why Choose Us */}
      <div className="bg-gray-50 py-16">
        <div className="max-w-6xl mx-auto px-4">
          <h2 className="text-3xl font-bold text-center mb-12">למה לבחור בנו?</h2>
          <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
            <div className="flex items-center gap-3">
              <CheckCircle className="w-6 h-6 text-blue-600 flex-shrink-0" />
              <div>
                <h3 className="font-bold mb-1">מקצועיות</h3>
                <p className="text-gray-600">שנים של ניסיון בתחום</p>
              </div>
            </div>
            <div className="flex items-center gap-3">
              <Clock className="w-6 h-6 text-blue-600 flex-shrink-0" />
              <div>
                <h3 className="font-bold mb-1">זמינות 24/7</h3>
                <p className="text-gray-600">שירות מהיר בכל שעה</p>
              </div>
            </div>
            <div className="flex items-center gap-3">
              <MapPin className="w-6 h-6 text-blue-600 flex-shrink-0" />
              <div>
                <h3 className="font-bold mb-1">שירות ארצי</h3>
                <p className="text-gray-600">הגעה לכל מקום</p>
              </div>
            </div>
            <div className="flex items-center gap-3">
              <CheckCircle className="w-6 h-6 text-blue-600 flex-shrink-0" />
              <div>
                <h3 className="font-bold mb-1">אמינות</h3>
                <p className="text-gray-600">שירות אמין ומקצועי</p>
              </div>
            </div>
          </div>
        </div>
      </div>

      {/* Contact */}
      <div className="max-w-6xl mx-auto px-4 py-16 text-center">
        <h2 className="text-3xl font-bold mb-8">צור קשר</h2>
        <div className="flex flex-col md:flex-row gap-6 justify-center items-center">
          <Button 
            size="lg"
            className="bg-blue-600 hover:bg-blue-700 text-lg gap-2 min-w-[200px] transform transition-transform hover:scale-105"
            onClick={() => window.location.href = 'tel:972555576780'}
          >
            <Phone className="w-5 h-5" />
            055-557-6780
          </Button>
          <Button 
            size="lg"
            className="bg-green-500 hover:bg-green-600 text-white text-lg gap-2 min-w-[200px] transform transition-transform hover:scale-105"
            onClick={() => window.location.href = whatsappLink}
          >
            <MessageCircle className="w-5 h-5" />
            WhatsApp
          </Button>
        </div>
      </div>

      {/* Footer */}
      <footer className="bg-gray-900 text-white py-8">
        <div className="max-w-6xl mx-auto px-4 text-center">
          <p>© {new Date().getFullYear()} בנימין מנעולן רכב - כל הזכויות שמורות</p>
        </div>
      </footer>
    </div>
  );
}
