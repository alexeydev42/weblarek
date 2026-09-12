# WebLarek

WebLarek is a TypeScript e-commerce application for browsing products, adding them to a cart and placing an order.

The project focuses on application architecture, API interaction and separation of responsibilities between data, presentation and coordination logic.

## Features

- product catalog loaded from an API;
- product details displayed in a modal window;
- shopping cart management;
- total price calculation;
- checkout flow;
- payment method and delivery information forms;
- form validation;
- order submission to the API.

## Architecture

The application follows an MVP-style architecture:

- **Model** — stores and manages application data;
- **View** — renders interface elements and handles user interaction;
- **Presenter** — coordinates models and views through application events.

An event-based approach is used to reduce direct dependencies between parts of the application and keep responsibilities separated.

## Tech stack

- TypeScript
- HTML
- SCSS
- Vite
- REST API

## Project structure

```text
src/
├── components/     UI components and base classes
├── types/          TypeScript types and interfaces
├── utils/          constants and utility functions
├── scss/           styles
└── main.ts         application entry point
```

## Getting started

Clone the repository and install dependencies:

```bash
git clone https://github.com/alexeydev42/weblarek.git
cd weblarek
npm install
```

Start the development server:

```bash
npm run dev
```

Production build:

```bash
npm run build
```

## About the project

This project was completed as part of the Yandex Practicum Frontend Developer program.

The main focus of my work was TypeScript application logic, API interaction, event-driven communication between application parts and structuring the project around an MVP-style architecture.
