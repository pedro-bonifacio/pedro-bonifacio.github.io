---
title: "Automating Used Car Search with a Raspberry Pi!"
excerpt: "Python-based web scraper that automatically monitors StandVirtual.<br/><br/><img src='/images/portfolio/standalert.jpg'><br/>"
collection: portfolio
---

# StandAlert: Automating Used Car Search with Python 🚗

Finding the perfect used car can be a time-consuming process, especially when you have specific criteria in mind. That's why I created [StandAlert](https://github.com/pedro-bonifacio/StandAlert), a Python-based web scraper that automatically monitors StandVirtual (a popular used car marketplace) and notifies you when new listings matching your criteria appear.

## The Problem

Anyone who has searched for a used car knows the drill: constantly refreshing listing pages, hoping to catch new postings before others. This manual process is:
- Time-consuming
- Prone to missing opportunities
- Inefficient, especially when monitoring multiple car models

## The Solution

StandAlert automates this entire process. It's designed to run continuously on a Raspberry Pi, checking for new listings every 30 minutes and sending email notifications when matches are found. Here's what makes it special:

### Key Features
- **Automated Monitoring**: Checks StandVirtual every 30 minutes (configurable interval)
- **Custom Filtering**: Users can define specific criteria through a simple CSV file
- **Email Notifications**: Instant alerts when new matching cars are listed
- **Raspberry Pi Optimized**: Runs efficiently in headless mode
- **Systemd Integration**: Can be set up as a system service for true automation

### Technical Implementation

The project leverages several technologies to achieve its goals:
- **Python** as the primary programming language
- **Selenium** with **ChromeDriver** for web scraping
- **Xvfb** for headless browser operation
- **Systemd** for service management
- **Gmail SMTP** for sending notifications

### Running as a Background Service

One of the most powerful features is the ability to run StandAlert as a systemd service. This means:
- Automatic startup on system boot
- Automatic restart on failures
- Easy log access through journalctl
- Proper service management through systemctl

## Lessons Learned

Building StandAlert taught me several valuable lessons:

1. **Web Scraping Best Practices**: Working with dynamic websites and handling different page states
2. **Service Management**: Setting up and maintaining long-running Python applications
3. **Automation**: Creating practical solutions for real-world problems
4. **Error Handling**: Ensuring robust operation in a continuous monitoring scenario

## Future Improvements

While StandAlert is fully functional, there's always room for enhancement:
- Adding support for more car marketplaces
- Implementing price trend analysis
- Creating a web interface for easier configuration
- Adding support for more notification methods (SMS, Push notifications)

## Conclusion

StandAlert demonstrates how programming can solve real-world problems and save time. It's a practical example of automation making our lives easier, one car search at a time. 

If you're interested in trying it out or contributing to the project, check out the [GitHub repository](https://github.com/pedro-bonifacio/StandAlert).

*Happy car hunting! 🚀*