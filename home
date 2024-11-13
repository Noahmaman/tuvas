import { useState } from 'react'
import { Button } from "@/components/ui/button"
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from "@/components/ui/card"
import { Input } from "@/components/ui/input"
import { Label } from "@/components/ui/label"
import { Tabs, TabsContent, TabsList, TabsTrigger } from "@/components/ui/tabs"
import { CalendarIcon, Globe, Leaf, Users, Zap, Home, Map, Search } from 'lucide-react'
import { Avatar, AvatarFallback, AvatarImage } from "@/components/ui/avatar"
import { Badge } from "@/components/ui/badge"

export default function NyxLandingPage() {
  const [activeTab, setActiveTab] = useState("explore")

  return (
    <div className="min-h-screen bg-white text-gray-900">
      {/* Header */}
      <header className="border-b">
        <div className="container mx-auto flex items-center justify-between px-4 py-4">
          <div className="text-2xl font-bold text-purple-600">Nyx</div>
          <nav className="hidden space-x-4 md:flex">
            <a href="#" className="text-sm font-medium hover:text-purple-600">Explore</a>
            <a href="#" className="text-sm font-medium hover:text-purple-600">Host</a>
            <a href="#" className="text-sm font-medium hover:text-purple-600">Sign Up</a>
            <a href="#" className="text-sm font-medium hover:text-purple-600">Log In</a>
          </nav>
        </div>
      </header>

      {/* Hero Section */}
      <section className="bg-gradient-to-r from-purple-100 to-blue-100 py-20">
        <div className="container mx-auto px-4">
          <h1 className="mb-6 text-4xl font-bold leading-tight md:text-5xl lg:text-6xl">
            Discover Sustainable <br /> Living Experiences
          </h1>
          <p className="mb-8 text-xl text-gray-700">
            Nyx reimagines travel with AI-powered recommendations and eco-friendly accommodations
          </p>
          <div className="rounded-lg bg-white p-4 shadow-lg md:inline-flex">
            <div className="mb-4 md:mb-0 md:mr-4">
              <Label htmlFor="location" className="mb-2 block text-sm font-medium">
                Where
              </Label>
              <Input id="location" placeholder="Anywhere" className="w-full md:w-64" />
            </div>
            <div className="mb-4 md:mb-0 md:mr-4">
              <Label htmlFor="check-in" className="mb-2 block text-sm font-medium">
                Check in
              </Label>
              <Input id="check-in" placeholder="Add dates" className="w-full md:w-40" />
            </div>
            <div className="mb-4 md:mb-0 md:mr-4">
              <Label htmlFor="check-out" className="mb-2 block text-sm font-medium">
                Check out
              </Label>
              <Input id="check-out" placeholder="Add dates" className="w-full md:w-40" />
            </div>
            <div>
              <Label htmlFor="guests" className="mb-2 block text-sm font-medium">
                Who
              </Label>
              <Input id="guests" placeholder="Add guests" className="w-full md:w-40" />
            </div>
            <Button size="lg" className="mt-4 w-full bg-purple-600 hover:bg-purple-700 md:mt-0 md:w-auto">
              <Search className="mr-2 h-4 w-4" /> Search
            </Button>
          </div>
        </div>
      </section>

      {/* Featured Experiences */}
      <section className="py-20">
        <div className="container mx-auto px-4">
          <h2 className="mb-12 text-center text-3xl font-bold">Featured Sustainable Experiences</h2>
          <div className="grid gap-8 md:grid-cols-2 lg:grid-cols-3">
            <ExperienceCard
              image="/placeholder.svg?height=400&width=600"
              title="Eco-Treehouse Retreat"
              location="Redwood National Park, CA"
              price={150}
              rating={4.9}
              reviews={128}
            />
            <ExperienceCard
              image="/placeholder.svg?height=400&width=600"
              title="Solar-Powered Beach Villa"
              location="Tulum, Mexico"
              price={200}
              rating={4.8}
              reviews={95}
            />
            <ExperienceCard
              image="/placeholder.svg?height=400&width=600"
              title="Off-Grid Mountain Cabin"
              location="Swiss Alps"
              price={180}
              rating={4.7}
              reviews={112}
            />
          </div>
        </div>
      </section>

      {/* Key Features */}
      <section className="bg-gray-100 py-20">
        <div className="container mx-auto px-4">
          <h2 className="mb-12 text-center text-3xl font-bold">Why Choose Nyx</h2>
          <div className="grid gap-8 md:grid-cols-2 lg:grid-cols-4">
            <FeatureCard
              icon={<Globe className="h-8 w-8 text-purple-600" />}
              title="AI-Powered Matching"
              description="Get personalized recommendations based on your preferences and travel patterns"
            />
            <FeatureCard
              icon={<Leaf className="h-8 w-8 text-green-600" />}
              title="Eco-Friendly Options"
              description="Discover and book sustainable accommodations with minimal environmental impact"
            />
            <FeatureCard
              icon={<Map className="h-8 w-8 text-blue-600" />}
              title="Virtual Exploration"
              description="Experience immersive virtual tours and augmented reality previews"
            />
            <FeatureCard
              icon={<Users className="h-8 w-8 text-indigo-600" />}
              title="Community-Driven"
              description="Join a decentralized ecosystem and participate in platform governance"
            />
          </div>
        </div>
      </section>

      {/* Immersive Exploration Showcase */}
      <section className="py-20">
        <div className="container mx-auto px-4">
          <h2 className="mb-8 text-center text-3xl font-bold">Immersive Exploration</h2>
          <Tabs value={activeTab} onValueChange={setActiveTab} className="w-full">
            <TabsList className="grid w-full grid-cols-2">
              <TabsTrigger value="explore">Virtual Tours</TabsTrigger>
              <TabsTrigger value="ar">Augmented Reality</TabsTrigger>
            </TabsList>
            <TabsContent value="explore" className="mt-4">
              <div className="aspect-video w-full overflow-hidden rounded-lg bg-gray-200">
                {/* Placeholder for Virtual Tour Demo */}
                <div className="flex h-full items-center justify-center">
                  <p className="text-xl">Interactive Virtual Tour Demo</p>
                </div>
              </div>
            </TabsContent>
            <TabsContent value="ar" className="mt-4">
              <div className="aspect-video w-full overflow-hidden rounded-lg bg-gray-200">
                {/* Placeholder for AR Demo */}
                <div className="flex h-full items-center justify-center">
                  <p className="text-xl">Augmented Reality Experience Demo</p>
                </div>
              </div>
            </TabsContent>
          </Tabs>
        </div>
      </section>

      {/* Testimonials */}
      <section className="bg-gray-100 py-20">
        <div className="container mx-auto px-4">
          <h2 className="mb-12 text-center text-3xl font-bold">What Our Users Say</h2>
          <div className="grid gap-8 md:grid-cols-2 lg:grid-cols-3">
            <TestimonialCard
              name="Alex Johnson"
              location="New York, USA"
              quote="Nyx has completely changed how I travel. The AI recommendations are spot-on, and I love supporting eco-friendly accommodations."
            />
            <TestimonialCard
              name="Maria Garcia"
              location="Barcelona, Spain"
              quote="The virtual tours feature is incredible. I felt like I was actually there before I even booked my stay!"
            />
            <TestimonialCard
              name="Yuki Tanaka"
              location="Tokyo, Japan"
              quote="As a host, I appreciate Nyx's focus on sustainability. It's helped me improve my property and attract conscious travelers."
            />
          </div>
        </div>
      </section>

      {/* Call-to-Action */}
      <section className="bg-purple-600 py-20 text-white">
        <div className="container mx-auto px-4 text-center">
          <h2 className="mb-6 text-3xl font-bold">Ready to Reimagine Travel?</h2>
          <p className="mb-8 text-xl">
            Join Nyx today and experience the future of sustainable, immersive accommodation booking.
          </p>
          <Button size="lg" className="bg-white text-purple-600 hover:bg-gray-100">
            Sign Up Now
          </Button>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-gray-900 py-8 text-white">
        <div className="container mx-auto px-4">
          <div className="grid gap-8 md:grid-cols-2 lg:grid-cols-4">
            <div>
              <h3 className="mb-4 text-lg font-semibold">About</h3>
              <ul className="space-y-2">
                <li><a href="#" className="hover:text-purple-400">How Nyx works</a></li>
                <li><a href="#" className="hover:text-purple-400">Newsroom</a></li>
                <li><a href="#" className="hover:text-purple-400">Investors</a></li>
                <li><a href="#" className="hover:text-purple-400">Careers</a></li>
              </ul>
            </div>
            <div>
              <h3 className="mb-4 text-lg font-semibold">Community</h3>
              <ul className="space-y-2">
                <li><a href="#" className="hover:text-purple-400">Diversity & Belonging</a></li>
                <li><a href="#" className="hover:text-purple-400">Sustainability</a></li>
                <li><a href="#" className="hover:text-purple-400">Nyx Associates</a></li>
                <li><a href="#" className="hover:text-purple-400">Nyx.org</a></li>
              </ul>
            </div>
            <div>
              <h3 className="mb-4 text-lg font-semibold">Host</h3>
              <ul className="space-y-2">
                <li><a href="#" className="hover:text-purple-400">Host your home</a></li>
                <li><a href="#" className="hover:text-purple-400">Host an experience</a></li>
                <li><a href="#" className="hover:text-purple-400">Responsible hosting</a></li>
                <li><a href="#" className="hover:text-purple-400">Resource Center</a></li>
              </ul>
            </div>
            <div>
              <h3 className="mb-4 text-lg font-semibold">Support</h3>
              <ul className="space-y-2">
                <li><a href="#" className="hover:text-purple-400">Help Center</a></li>
                <li><a href="#" className="hover:text-purple-400">Cancellation options</a></li>
                <li><a href="#" className="hover:text-purple-400">Neighborhood Support</a></li>
                <li><a href="#" className="hover:text-purple-400">Trust & Safety</a></li>
              </ul>
            </div>
          </div>
          <div className="mt-8 border-t border-gray-700 pt-8 text-center">
            <p>&copy; 2024 Nyx, Inc. All rights reserved.</p>
          </div>
        </div>
      </footer>
    </div>
  )
}

function ExperienceCard({ image, title, location, price, rating, reviews }) {
  return (
    <Card className="overflow-hidden">
      <img src={image} alt={title} className="h-48 w-full object-cover" />
      <CardContent className="p-4">
        <h3 className="mb-2 text-lg font-semibold">{title}</h3>
        <p className="mb-2 text-sm text-gray-600">{location}</p>
        <div className="flex items-center justify-between">
          <p className="font-semibold">${price} / night</p>
          <div className="flex items-center">
            <span className="mr-1 text-yellow-500">★</span>
            <span>{rating}</span>
            <span className="ml-1 text-sm text-gray-600">({reviews})</span>
          </div>
        </div>
      </CardContent>
    </Card>
  )
}

function FeatureCard({ icon, title, description }) {
  return (
    <Card>
      <CardHeader>
        <div className="mb-2">{icon}</div>
        <CardTitle>{title}</CardTitle>
      </CardHeader>
      <CardContent>
        <CardDescription>{description}</CardDescription>
      </CardContent>
    </Card>
  )
}

function TestimonialCard({ name, location, quote }) {
  return (
    <Card>
      <CardContent className="p-6">
        <div className="mb-4 flex items-center">
          <Avatar className="mr-4">
            <AvatarImage src="/placeholder.svg" alt={name} />
            <AvatarFallback>{name.split(' ').map(n => n[0]).join('')}</AvatarFallback>
          </Avatar>
          <div>
            <h3 className="font-semibold">{name}</h3>
            <p className="text-sm text-gray-600">{location}</p>
          </div>
        </div>
        <p className="italic">"{quote}"</p>
      </CardContent>
    </Card>
  )
}
