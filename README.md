/** @type {import('next').NextConfig} */

const repoName = "REPO-NAME"

const nextConfig = {
  output: "export",
  basePath: `/${repoName}`,
  assetPrefix: `/${repoName}/`,
  trailingSlash: true,
  images: {
    unoptimized: true
  }
}

module.exports = nextConfig
/** @type {import('next').NextConfig} */

const repoName = "REPO-NAME"  // 🔴 Replace with your GitHub repo name

const nextConfig = {
  output: "export",
  basePath: `/${repoName}`,
  assetPrefix: `/${repoName}/`,
  trailingSlash: true,
  images: {
    unoptimized: true
  }
}

module.exports = nextConfig
import Hero from "../pages/home/components/Hero"
import GameSection from "../pages/home/components/GameSection"
import ControlsSection from "../pages/home/components/ControlsSection"
import Footer from "../pages/home/components/Footer"

export default function HomePage() {
  return (
    <main>
      <Hero />
      <GameSection />
      <ControlsSection />
      <Footer />
    </main>
  )
}
{
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "export": "next export",
    "deploy": "gh-pages -d out"
  }
}
