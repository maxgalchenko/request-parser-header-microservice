# Request Header Parser Microservice

<div align="center">

[![Node.js](https://img.shields.io/badge/Node.js-15.2.1-339933?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![Express](https://img.shields.io/badge/Express-5%20alpha-black?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![CORS](https://img.shields.io/badge/CORS-Enabled-blue?style=for-the-badge)](#)

</div>

## Overview

A minimal Express microservice for the freeCodeCamp Request Header Parser project. It returns the client's IP address, preferred language, and user agent as JSON.

## Key Features

- `GET /api/whoami` returns `ipaddress`, `language`, and `software` from request headers
- CORS enabled for broad compatibility
- Serves static assets from `build/` for a simple UI

## Tech Stack

Node.js 15, Express 5 (alpha), CORS

## Architecture

Lightweight Express server with a single JSON endpoint (`/api/whoami`) and static file serving from `build/`. Designed to run behind a reverse proxy where `x-forwarded-for` is set.

## Performance & Accessibility

Minimal middleware and fast JSON responses; suitable for small footprint deployments. Accessibility considerations are handled by any client consuming this API.

## Prerequisites

- Node.js: `15.2.1`

## Installation

```bash
git clone https://github.com/maxgalchenko/request-parser-header-microservice.git
cd request-parser-header-microservice
npm install
```

## Environment Variables

```env
PORT=3000
```

## Quick Start

```bash
export PORT=3000
npm start
```

Open http://localhost:3000

## Available Scripts

- `npm start` – Start the Express server on `PORT`.

---

<div align="center">

Built with ❤️ by [Maksym Galchenko](https://github.com/maxgalchenko)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/galchenko-max/)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-green?style=for-the-badge&logo=web)](https://portfolio-green-six-29.vercel.app/)
[![Email](https://img.shields.io/badge/Email-Contact-red?style=for-the-badge&logo=gmail)](mailto:galchenko.maksym@gmail.com)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

</div>
