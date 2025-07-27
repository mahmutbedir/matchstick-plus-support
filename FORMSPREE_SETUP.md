# Formspree Setup Guide

## What is Formspree?

Formspree is a free form handling service that allows you to collect form submissions via email without any backend code. Perfect for static sites like GitHub Pages.

## Setup Instructions

### 1. Create Formspree Account
1. Go to [formspree.io](https://formspree.io)
2. Sign up for a free account
3. Verify your email address

### 2. Create a New Form
1. Click "New Form" in your dashboard
2. Give your form a name (e.g., "CopyBridge Support")
3. Copy the form ID (it will look like: `xrgjqkab`)

### 3. Update the HTML
Replace `YOUR_FORM_ID` in the `index.html` file with your actual form ID:

```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" class="contact-form">
```

Example:
```html
<form action="https://formspree.io/f/xrgjqkab" method="POST" class="contact-form">
```

### 4. Test the Form
1. Deploy your site to GitHub Pages
2. Fill out and submit the form
3. Check your email for the submission
4. Check your Formspree dashboard for the submission

## Features

✅ **Free Plan**: 50 submissions per month  
✅ **Email Notifications**: Get notified instantly  
✅ **Spam Protection**: Built-in spam filtering  
✅ **No Backend Required**: Works with static sites  
✅ **Easy Setup**: Just change the form action URL  

## Form Fields

The current form includes:
- **Name**: User's full name
- **Email**: User's email address
- **Subject**: Message subject/title
- **Message**: Detailed message content

## Customization

You can easily modify the form fields by:
1. Adding/removing form groups in HTML
2. Updating the CSS styles
3. Modifying validation in JavaScript

## Alternative Services

If you need more features, consider:
- **Netlify Forms**: More submissions, better integration
- **Google Forms**: Free, unlimited submissions
- **Typeform**: Professional forms with advanced features

## Troubleshooting

**Form not sending?**
- Check if the form ID is correct
- Verify your email is confirmed in Formspree
- Check browser console for errors

**Not receiving emails?**
- Check spam folder
- Verify email address in Formspree settings
- Check Formspree dashboard for submissions 