# Introduction

Markdown is an easy-to-read, easy-to-write language for formatting plain text. You can use Markdown syntax, along with some additional HTML tags, to format your writing on GitHub, in places like repository READMEs and comments on pull requests and issues. In this guide, you'll learn some advanced formatting features by creating or editing a README for your GitHub profile.

If you're new to Markdown, you might want to start with "Basic writing and formatting syntax" or the Communicate using Markdown GitHub Skills course.

# Creating or editing your profile README

Your profile README lets you share information about yourself with the community on GitHub.com. The README is displayed at the top of your profile page.

If you don't already have a profile README, you can add one.

- Create a repository with the same name as your GitHub username, initializing the repository with a README.md file. For more information, see "Managing your profile README."
- Edit the README.md file and delete the template text (beginning ### Hi there) that is automatically added when you create the file.
- If you already have a profile README, you can edit it from your profile page.

# Adding an image to suit your visitors

You can include images in your communication on GitHub. Here, you'll add a responsive image, such as a banner, to the top of your profile README.

By using the HTML <picture> element with the prefers-color-scheme media feature, you can add an image that changes depending on whether a visitor is using light or dark mode. For more information, see "Managing your theme settings."

Copy and paste the following markup into your README.md file.

<picture>
 <source media="(prefers-color-scheme: dark)" srcset="YOUR-DARKMODE-IMAGE">
 <source media="(prefers-color-scheme: light)" srcset="YOUR-LIGHTMODE-IMAGE">
 <img alt="YOUR-ALT-TEXT" src="YOUR-DEFAULT-IMAGE">
</picture>

| Rank | THING-TO-RANK |
|-----:|---------------|
|     1|               |
|     2|               |
|     3|               |
