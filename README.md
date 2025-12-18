# Nano Banana Pro

A free, open-source AI image generator and editor powered by Google Gemini 2.5 Flash Image. Create stunning images from text prompts, edit existing images with AI, and explore multiple aspect ratios—all in a modern, intuitive interface.

[![Built with v0](https://img.shields.io/badge/Built%20with-v0.app-black?style=for-the-badge)](https://v0.app/templates/nano-banana-pro-playground-hkRpZoLOrJC)

## Features

- **Text-to-Image Generation**: Create images from natural language descriptions
- **Image Editing**: Upload and transform existing images using AI
- **Multi-Image Input**: Combine multiple images in your generation
- **Aspect Ratio Control**: Support for various aspect ratios (square, portrait, landscape)
- **HEIC Conversion**: Automatic conversion of HEIC images to compatible formats
- **Generation History**: Persistent history of your creations with local storage
- **URL-Based Input**: Load images from URLs for quick editing
- **Fullscreen Viewer**: View generated images in fullscreen mode
- **Dark Mode**: Full theme support for comfortable viewing
- **Mobile Responsive**: Optimized experience across all devices

## Tech Stack

- **Framework**: [Next.js 16](https://nextjs.org/) with React 19
- **AI Model**: Google Gemini 2.5 Flash Image via [Vercel AI SDK](https://sdk.vercel.ai/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) with custom animations
- **UI Components**: [Radix UI](https://www.radix-ui.com/) primitives
- **Type Safety**: TypeScript with Zod validation
- **Image Processing**: HEIC conversion and client-side processing

## Getting Started

### Prerequisites

- Node.js 18+ and npm/yarn/pnpm
- Google AI API key ([Get one here](https://aistudio.google.com/apikey))

### Installation

1. Clone the repository:
```bash
git clone https://github.com/feraandrei1/vercel-v0-nano-banana-photo-generator
cd vercel-v0-nano-banana-photo-generator-main
```

2. Install dependencies:
```bash
npm install
# or
yarn install
# or
pnpm install
```

3. Create a `.env.local` file in the root directory:
```env
GOOGLE_GENERATIVE_AI_API_KEY=your_api_key_here
```

4. Run the development server:
```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `GOOGLE_GENERATIVE_AI_API_KEY` | Your Google Gemini API key | Yes |

## Usage

1. **Generate from text**: Enter a prompt describing the image you want to create
2. **Upload images**: Drag and drop or click to upload reference images
3. **Choose aspect ratio**: Select your preferred output dimensions
4. **Generate**: Click the generate button and wait for your AI-created image
5. **View history**: Browse your previous generations in the history panel
6. **Load to editor**: Click any historical image to load it back into the editor

## Project Structure

```
├── app/                    # Next.js app directory
│   ├── api/               # API routes for image generation
│   ├── layout.tsx         # Root layout with theme provider
│   └── page.tsx           # Main page component
├── components/            # React components
│   ├── image-combiner/    # Main image generation UI
│   └── ui/                # Reusable UI components
├── hooks/                 # Custom React hooks
├── lib/                   # Utility functions
└── public/                # Static assets
```

## Deployment

This project is optimized for deployment on [Vercel](https://vercel.com):

1. Push your code to GitHub
2. Import the project in Vercel
3. Add your environment variables
4. Deploy

## Based on v0 Template

This project is built from the [Nano Banana Pro Playground](https://v0.app/templates/nano-banana-pro-playground-hkRpZoLOrJC) template from v0.app, featuring automatic sync with v0 deployments.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Powered by [Google Gemini 2.5 Flash Image](https://ai.google.dev/)
- Built with [v0.app](https://v0.app)
- UI components from [Radix UI](https://www.radix-ui.com/)
- Deployed on [Vercel](https://vercel.com)
