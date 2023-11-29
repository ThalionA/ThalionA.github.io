---
layout: default
title: Contact Us
---

<style>
    /* Container holding the form */
    .contact-form {
        max-width: 600px;
        margin: 0 auto;
        padding: 1em;
        background: #f9f9f9;
        border-radius: 5px;
    }

    /* Style inputs, textarea, and button */
    .contact-form input[type="text"],
    .contact-form input[type="email"],
    .contact-form textarea {
        width: 100%;
        padding: 0.5em;
        margin-bottom: 1em;
        border: 1px solid #ccc;
        border-radius: 3px;
    }

    .contact-form textarea {
        height: 150px;
    }

    .contact-form button {
        background: #007bff;
        color: white;
        border: none;
        padding: 0.7em 1.5em;
        text-transform: uppercase;
        cursor: pointer;
        border-radius: 3px;
        display: block;
        width: 100%;
    }

    .contact-form button:hover {
        background: #0056b3;
    }

    /* Label styling */
    .contact-form label {
        display: block;
        margin-bottom: .5em;
    }

    /* Focus styles for input elements */
    .contact-form input:focus,
    .contact-form textarea:focus {
        outline: none;
        border-color: #007bff;
    }
</style>

## How to contact us

<div class="contact-form">
    <form action="https://formspree.io/f/xgejjngl" method="POST">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">Email:</label>
        <input type="email" id="email" name="_replyto" required>

        <label for="message">Message:</label>
        <textarea id="message" name="message" required></textarea>

        <!-- Hidden input to help prevent spam -->
        <input type="text" name="_gotcha" style="display:none">

        <button type="submit">Send</button>
    </form>
</div>
