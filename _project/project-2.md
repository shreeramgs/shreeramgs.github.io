---
title: "E-Wal Digital Wallet"
excerpt: "Full-stack payment web application with user authentication, wallet management, fund transfers, and admin dashboard. Built with Node.js, Express, and MySQL."
collection: project
image: "/images/Ewal.png"
tags:
  - Node.js
  - MySQL
  - Express
  - Full-Stack
github: "https://github.com/shreeramgs/E-wal"
demo: "https://github.com/shreeramgs/E-wal"
---

<div style="display: flex; justify-content: center; margin-bottom: 2em;">
  <div 
    style="
      background: #fff;
      border-radius: 16px;
      box-shadow: 0 2px 8px 0 rgba(0,0,0,0.12);
      padding: 1.2em 1.2em 1em 1.2em;
      max-width: 520px;
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
    "
  >
    <img 
      id="ewal-slider-img"
      src="/images/Ewal_1.png" 
      alt="E-Wal Digital Wallet" 
      style="max-width: 440px; width: 90%; aspect-ratio: 16/10; height: auto; object-fit: contain; border-radius: 12px; box-shadow: 0 2px 8px 0 rgba(0,0,0,0.10); margin-bottom: 0.4em; transition: transform 0.38s cubic-bezier(.21,.8,.38,1.01), opacity 0.38s cubic-bezier(.21,.8,.38,1.01);"
    />
  </div>
</div>
<script>
(function() {
  const images = [
    "/images/Ewal_1.png",
    "/images/Ewal_2.png",
    "/images/Ewal_3.png",
    "/images/Ewal.png"
  ];
  let idx = 0;
  let transitioning = false;

  function preloadImages(arr) {
    arr.forEach(src => {
      const img = new window.Image();
      img.src = src;
    });
  }

  function animateSlide(img, nextSrc) {
    if (!img) return;
    transitioning = true;

    // Smoother, slightly faster in-out zoom
    img.style.transition = 'transform 0.37s cubic-bezier(.36,.57,.75,.68), opacity 0.37s cubic-bezier(.36,.57,.75,.68)';
    img.style.transform = 'scale(.95)';
    img.style.opacity = 0;

    setTimeout(() => {
      img.src = nextSrc;
      img.style.transition = 'none';
      img.style.transform = 'scale(1.04)';
      setTimeout(() => {
        img.style.transition = 'transform 0.38s cubic-bezier(.21,.8,.38,1.01), opacity 0.38s cubic-bezier(.21,.8,.38,1.01)';
        img.style.transform = 'scale(1)';
        img.style.opacity = 1;
        setTimeout(() => {
          transitioning = false;
        }, 420);
      }, 18);
    }, 230);
  }

  function changeImage() {
    if (transitioning) return;
    const img = document.getElementById('ewal-slider-img');
    if (!img) return;
    idx = (idx + 1) % images.length;
    animateSlide(img, images[idx]);
  }

  document.addEventListener('DOMContentLoaded', function() {
    preloadImages(images);
    if (images.length > 1) {
      setInterval(changeImage, 2300);
    }
  });
})();
</script>

**E-Wal** is a prototype web application that enables users to conveniently manage money on the go. With E-Wal, you can easily store and manage your money, pay bills, and make online purchases without the need for cash or cards.

## Features

- **Instant Access**: Make transactions with just a few clicks, anytime, anywhere
- **Bank Linking**: Link your bank accounts for seamless transfers
- **P2P Transfers**: Transfer funds to other users or receive money
- **Transaction Tracking**: View account balance and manage your budget

## Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MySQL
- **Frontend**: HTML, CSS, JavaScript, Materialize Framework
- **Authentication**: Express-session, Cookie-parser

## User Features

- Dashboard with account overview
- Profile management
- Wallet with add/request money
- Fund transfer between users
- Transaction history

## Admin Features

- Monitor user accounts
- View total active users
- Access complete transaction history
- Add other administrators
