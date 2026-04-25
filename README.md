
# Khuli Canvas: A Social Storytelling & E-commerce Platform

## Overview

**Khuli Canvas** is a full-stack web application designed to be a vibrant and inclusive space for creative expression. At its core, it's a social platform where users can write, share, and discover stories, either openly or anonymously. It fosters a supportive community through features like following, liking, and commenting.

Beyond social storytelling, Khuli Canvas integrates a complete e-commerce solution, allowing administrators to manage and sell products through a beautiful, customizable storefront. The platform is further enhanced by a suite of powerful AI tools, powered by Google's Gemini through Genkit, which assist both users in their creative process and administrators in content management.

This project is built on a modern, robust technology stack, providing a seamless, performant, and feature-rich experience for users and a powerful, intuitive control panel for administrators.


---

## Key Features

### I. User-Facing Features

#### 1. Authentication & Onboarding
- **Comprehensive Registration Flow**: A guided, multi-step process for new users:
    1.  **Basic Information**: Full name, unique username, email, and password.
    2.  **Profile Images**: Upload or use AI to generate an avatar and a cover image.
    3.  **Category Selection**: Users pick their interests (e.g., Love, Confession, Poetry) to personalize their feed.
    4.  **Profile Completion**: Add a bio, social links, and set personal content preferences.
- **Email & Password Login**: Secure and standard login method.
- **Anonymous Browsing**: Users can explore the platform and read public stories without creating an account.

#### 2. Social & Community
- **Personalized Dashboard**: The main feed displays stories from followed users and recommended content based on selected interests.
- **User Profiles**: Each user has a customizable profile page featuring their bio, stories, follower/following count, and social links.
- **Follow System**: Users can follow each other to see their latest stories in their feed.
- **Notifications**: A real-time notification system alerts users to new followers, follow requests, likes, comments, and administrative actions.
- **Interactive Story Feed**: Users can like, comment on, and save (bookmark) stories.
- **Inbox & Direct Messaging**: A complete real-time chat system for one-on-one or group conversations.

#### 3. Story Creation & Consumption
- **Multi-Step Story Creator**: A sophisticated and user-friendly editor for crafting stories.
    - **Block-Based Canvas**: Build stories with various content types: paragraphs, headings, images, quotes, galleries, embedded links, and interactive polls.
    - **Text Styling**: Customize text with different fonts, colors, and styles (bold, italic).
    - **AI Assistance**:
        - **Story Generation**: Generate a full story with images from a simple prompt.
        - **Title Suggestions**: Get catchy, AI-generated titles based on the story's description.
- **Multiple Privacy Levels**:
    - **Public**: Visible to everyone and linked to the user's profile.
    - **Anonymous**: Visible to everyone but not linked to the user's profile.
    - **Private**: Visible only to the user on their own profile.
    - **Direct**: Can be shared only with specific users via direct message.
- **Immersive Story Viewer**: A beautifully designed page for reading stories, complete with author information, engagement actions, and related stories.

#### 4. E-commerce Storefront
- **Shop Onboarding & Home Page**: A visually engaging landing page with promotional banners, featured categories, and curated product sections.
- **Product Discovery**:
    - **All Products Page**: A filterable and sortable view of all available products.
    - **Category Pages**: Browse products within specific categories.
    - **Detailed Product Page**: View product images, descriptions, specifications, pricing, and user reviews.
- **Shopping Cart & Checkout**:
    - A persistent shopping cart accessible via a slide-in sidebar.
    - Support for applying discount coupons.
    - A multi-step checkout process (Address -> Payment).
    - "Cash on Delivery" as the initial payment method.
- **Wishlist**: Users can save their favorite products to a personal wishlist.
- **Order Tracking**: A dedicated section for users to view their order history and track the status of current orders (Pending, Processing, Shipped, Delivered).

---

### II. Admin Panel Features

The application includes a secure, comprehensive admin panel accessible only to the designated administrator.

#### 1. Dashboard & Analytics
- **At-a-Glance Overview**: The main dashboard provides key metrics, including total users, stories, flagged reports, and AI usage stats.
- **Data Visualizations**: Interactive charts display new user sign-ups and the distribution of story privacy types.
- **Quick-Access Links**: Cards linking to major content management sections.

#### 2. Social & Content Management
- **User Management**:
    - View, search, and filter all registered users.
    - **Detailed User View**: Inspect a user's profile, stories, followers, saved items, and account status.
    - **Moderation Actions**:
        - **Warn**: Send an official warning notification to a user.
        - **Suspend**: Temporarily suspend a user's account for a specified duration.
        - **Delete**: Remove a user's profile.
    - **Data Export**: Export user data to a PDF with customizable columns.
- **Story Moderation**: A unified view of all stories (public, anonymous, direct) with options to view, feature, or delete any story.
- **Blog Management**:
    - **AI-Powered Blog Editor**: Create and edit full blog posts using a block-based editor. Generate entire posts, including titles, sections, and featured image prompts, from a single idea.
    - **Post Management**: View all blog posts, check their status (Draft/Published), and manage them.
- **Explore Page Management**:
    - **Banners**: Create, edit, and delete promotional banners for the Explore page, with AI assistance for title and image generation.
    - **Categories**: Manage story categories, including their icons and images, with AI generation tools.
    - **Featured Content**: Hand-pick stories and users to feature on the Explore page.

#### 3. E-commerce Management
- **Product Management**:
    - **Full Product CRUD**: Create, read, update, and delete products.
    - **AI Product Generator**: Generate a complete product listing—including name, descriptions, pricing, specifications, and a main image—from a single prompt.
    - **AI Image Tools**: Generate main and gallery images using AI, with suggestions based on the product image.
    - **Advanced Filtering & Views**: Manage products in a list or grid view with powerful filtering and search capabilities.
- **Order Management**:
    - View all customer orders with status, date, and total.
    - **Detailed Order View**: Inspect individual orders, see customer details, shipping address, and the full pricing breakdown (including discounts).
    - **Status Updates**: Update the status of an order (Pending, Processing, Shipped, Delivered).
- **Discount & Coupon Management**: Create, edit, and manage percentage-based or fixed-amount discount coupons with expiry dates and minimum order values.
- **Shop Customization**:
    - **Onboarding Screen**: Edit the initial welcome screen for the shop.
    - **Landing Page Editor**: A drag-and-drop interface to build the shop's home page by arranging banners, categories, and curated product sections.

---

## Technology Stack

- **Frontend**:
    - **Framework**: Next.js 14 with App Router
    - **UI**: React 18, TypeScript, ShadCN UI
    - **Styling**: Tailwind CSS
    - **State Management**: Zustand
    - **Animation**: Framer Motion
- **Backend & Database**:
    - **Platform**: Firebase
    - **Authentication**: Firebase Authentication
    - **Database**: Firestore (NoSQL)
- **Generative AI**:
    - **Platform**: Genkit (Google AI)
    - **Model**: Gemini (for text and image generation)
- **Deployment**:
    - **Hosting**: Firebase App Hosting
- **DevOps**:
    - Integrated with Firebase Studio for conversational development and rapid prototyping.
- **Utilities**:
    - **Image Hosting**: Cloudinary
    - **Forms**: React Hook Form with Zod for validation

This combination of technologies ensures a highly performant, scalable, and maintainable application with a cutting-edge, AI-enhanced feature set.
