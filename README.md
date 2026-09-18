# WebLarek

WebLarek is a TypeScript e-commerce application for browsing products, adding them to a cart and placing an order.

The project is mainly about architecture: separating data, UI and coordination logic, keeping dependencies controlled and organizing the application around an MVP-style approach.

<!-- TODO: Add 1 screenshot here: the product catalog with the cart or checkout flow visible. -->

## Key features

- product catalog loaded from an API;
- product details in a modal window;
- shopping cart management;
- total price calculation;
- checkout flow;
- payment and delivery forms;
- form validation;
- order submission to the API.

## Architecture

The application follows an MVP-style structure:

- **Model** stores and manages application data;
- **View** renders interface elements and handles user interaction;
- **Presenter** coordinates models and views through application events.

An event-based approach reduces direct dependencies between parts of the application and keeps responsibilities separated.

## What this project demonstrates

The main value of the project is not the number of screens, but the way the code is structured.

I used TypeScript types and interfaces to define data contracts, separated reusable UI classes from application data, and connected parts of the application through events rather than tightly coupling components to each other.

This made the checkout flow, cart updates and product state easier to reason about and extend.

## Tech stack

- TypeScript
- HTML
- SCSS
- Vite
- REST API

## Project structure

```text
src/
├── components/  # UI components and base classes
├── types/       # TypeScript types and interfaces
├── utils/       # constants and utility functions
├── scss/        # styles
└── main.ts      # application entry point
```

## Run locally

```bash
git clone https://github.com/alexeydev42/weblarek.git
cd weblarek
npm install
npm run dev
```

Production build:

```bash
npm run build
```

## Project context

This project was completed as part of the Yandex Practicum Frontend Developer program. My work focused on TypeScript application logic, API interaction, event-driven communication and the separation of responsibilities between application layers.
