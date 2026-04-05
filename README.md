<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Built by Brooklyn — Remote Softball Coaching</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=DM+Sans:ital,wght@0,300;0,400;0,500;1,300&display=swap" rel="stylesheet" />
  <style>
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    :root {
      --navy: #0C1B33;
      --navy-alt: #0a1628;
      --navy-dark: #060f1e;
      --orange: #E8512A;
      --cream: #F5EFE4;
      --gold: #C9A96E;
      --white: #FFFFFF;
      --muted: rgba(245,239,228,0.55);
      --ff-head: 'Bebas Neue', sans-serif;
      --ff-body: 'DM Sans', sans-serif;
    }

    html {
      background-color: #0C1B33 !important;
      scroll-behavior: smooth;
    }

    body {
      background-color: #0C1B33 !important;
      color: var(--cream);
      font-family: var(--ff-body);
      font-weight: 300;
      overflow-x: hidden;
    }

    a {
      color: inherit;
    }

    nav {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      z-index: 1000;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1.2rem 3rem;
      background: rgba(12,27,51,0.88);
      backdrop-filter: blur(14px);
      border-bottom: 1px solid rgba(232,81,42,0.2);
    }

    .nav-logo {
      font-family: var(--ff-head);
      font-size: 1.6rem;
      letter-spacing: 0.08em;
      color: var(--orange);
      text-decoration: none;
      white-space: nowrap;
    }

    .nav-links {
      list-style: none;
      display: flex;
      align-items: center;
      gap: 2.5rem;
    }

    .nav-links a {
      color: var(--cream);
      text-decoration: none;
      font-size: 0.85rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      font-weight: 400;
      opacity: 0.75;
      transition: opacity 0.2s, color 0.2s, background 0.2s;
    }

    .nav-links a:hover {
      opacity: 1;
      color: var(--orange);
    }

    .nav-cta {
      background: var(--orange);
      color: var(--white) !important;
      opacity: 1 !important;
      padding: 0.55rem 1.4rem;
      border-radius: 2px;
    }

    .nav-cta:hover {
      background: #c63f1b;
      color: var(--white) !important;
    }

    section {
      padding: 7rem 3rem;
      background-color: var(--navy);
    }

    .section-label {
      font-size: 0.72rem;
      letter-spacing: 0.3em;
      text-transform: uppercase;
      color: var(--orange);
      margin-bottom: 1rem;
    }

    .section-title {
      font-family: var(--ff-head);
      font-size: clamp(2.8rem, 5vw, 5rem);
      line-height: 1;
      color: var(--white);
      margin-bottom: 1.5rem;
    }

    .section-sub {
      font-size: 1rem;
      line-height: 1.75;
      color: var(--cream);
      opacity: 0.75;
      max-width: 560px;
    }

    .btn-primary,
    .btn-ghost,
    .btn-submit {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      text-decoration: none;
      border-radius: 2px;
      font-family: var(--ff-body);
      font-size: 0.85rem;
      font-weight: 500;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      cursor: pointer;
      transition: background 0.2s, color 0.2s, border-color 0.2s, transform 0.15s;
    }

    .btn-primary:hover,
    .btn-ghost:hover,
    .btn-submit:hover {
      transform: translateY(-2px);
    }

    .btn-primary {
      background: var(--orange);
      color: var(--white);
      padding: 0.9rem 2.2rem;
      border: none;
    }

    .btn-primary:hover {
      background: #c63f1b;
    }

    .btn-ghost {
      background: transparent;
      color: var(--cream);
      padding: 0.9rem 2.2rem;
      border: 1px solid rgba(245,239,228,0.35);
    }

    .btn-ghost:hover {
      color: var(--orange);
      border-color: var(--orange);
    }

    #hero {
      background-color: var(--navy);
      min-height: 100vh;
      display: grid;
      grid-template-columns: 1fr 1fr;
      overflow: hidden;
      padding: 0;
    }

    .hero-left {
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 9rem 4rem 6rem 3rem;
      position: relative;
      z-index: 2;
      background-color: var(--navy);
    }

    .hero-eyebrow,
    .hero-title,
    .hero-sub,
    .hero-btns,
    .hero-stat-badge {
      opacity: 0;
      animation-fill-mode: forwards;
    }

    .hero-eyebrow {
      font-size: 0.75rem;
      letter-spacing: 0.25em;
      text-transform: uppercase;
      color: var(--orange);
      margin-bottom: 1.2rem;
      animation: fadeUp 0.7s 0.2s forwards;
    }

    .hero-title {
      font-family: var(--ff-head);
      font-size: clamp(4.5rem, 8vw, 8rem);
      line-height: 0.92;
      color: var(--white);
      margin-bottom: 1.8rem;
      animation: fadeUp 0.8s 0.4s forwards;
    }

    .hero-title span {
      display: block;
      color: var(--orange);
    }

    .hero-sub {
      font-size: 1.05rem;
      line-height: 1.7;
      color: var(--cream);
      max-width: 420px;
      margin-bottom: 2.8rem;
      animation: fadeUp 0.8s 0.6s forwards;
    }

    .hero-btns {
      display: flex;
      gap: 1rem;
      flex-wrap: wrap;
      animation: fadeUp 0.8s 0.8s forwards;
    }

    .hero-right {
      position: relative;
      display: flex;
      align-items: cen
