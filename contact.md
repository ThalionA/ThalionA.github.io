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
        border-radius: 70%; /* This will create the circular effect */
        text-align: center;
        overflow: hidden; /* This ensures no inner content spills out of the circular bounds */
    }

    /* Additional styles might be necessary for form elements */
    .contact-form input[type="text"],
    .contact-form input[type="email"],
    .contact-form textarea,
    .contact-form button {
        /* Assuming you want these elements to keep straight edges */
        border-radius: 0; /* Resets any border-radius applied to form elements */
        /* Other styles... */
    }

    /* You might want to adjust the form elements to ensure they fit well within the circular container */
    .contact-form input[type="text"],
    .contact-form input[type="email"],
    .contact-form textarea {
        width: calc(100% - 2em); /* Adjust width considering padding */
        margin: 0.5em auto; /* Centering the inputs */
        display: block;
    }

    .contact-form button {
        /* Other styles... */
        margin-top: 0.5em;
    }

    /* Adjust the height of the textarea for better fit */
    .contact-form textarea {
        height: 100px; /* Example height */
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
