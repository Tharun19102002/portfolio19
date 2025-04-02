# Serverless Portfolio Website


This project is a modern, interactive portfolio website deployed on AWS S3 for serverless hosting. It showcases my skills, projects, and experience as a Cloud Engineer and DevOps Practitioner with eye-catching animations and responsive design.

## Demo Site

Visit the live portfolio: [http://myportfolio1910.s3-website.eu-north-1.amazonaws.com/](http://myportfolio1910.s3-website.eu-north-1.amazonaws.com/)

|  ![Portfolio Home]("C:\Users\tharu\OneDrive\Pictures\Screenshots\Portfolio SS-1.png") | ![Portfolio Projects]("C:\Users\tharu\OneDrive\Pictures\Screenshots\Portfolio SS-1.png") |
|---|---|

## Features

- **Interactive Cloud Background**: Dynamic animated cloud background using Vanta.js
- **Smooth Animations**: Page elements animate on scroll using GSAP
- **Responsive Design**: Fully responsive layout works on all devices
- **Navigation**: Smooth scrolling navigation with fixed header
- **Modern UI**: Clean design with cards, hover effects, and transitions
- **AWS Hosted**: Deployed on AWS S3 for serverless, scalable hosting

## Technologies Used

```
HTML5
CSS3
JavaScript
Vanta.js - For animated backgrounds
GSAP - For smooth animations
Font Awesome - For icons
Google Fonts - Poppins font family
AWS S3 - For static website hosting
```

## AWS Integration

The portfolio website is deployed using AWS services:

- **S3**: Static website hosting with public access
- **CloudFront** (optional): Content delivery for global performance
- **Route 53** (optional): Domain management
- **Certificate Manager** (optional): SSL/TLS certificate

## Implementation Details

- **Serverless Architecture**: No server management required
- **Cost-Effective**: Uses AWS free tier resources where possible
- **Scalable**: Automatically handles traffic spikes
- **High Availability**: Distributed across multiple AWS availability zones

## Project Structure

```
portfolio-website/
├── index.html               # Main HTML file with embedded CSS and JS
├── assets/                  # Directory for images and other assets
│   └── THARUN_PHOTO.jpg     # Profile photo
├── README.md                # Project documentation
└── LICENSE                  # License information
```

## Setup and Deployment

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/Tharun19102002/portfolio-website.git
cd portfolio-website
```

2. Open `index.html` in your browser or use a local server:
```bash
# Using Python's built-in server
python -m http.server

# Or with Node.js
npx serve
```

### AWS S3 Deployment

1. Create an S3 bucket with static website hosting enabled
2. Set the bucket policy for public access:
```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-bucket-name/*"
    }
  ]
}
```
3. Upload all files to the bucket
4. Configure the static website hosting in bucket properties

## Future Enhancements

- Add a blog section with AWS Lambda backend
- Implement Contact Form with API Gateway and Lambda
- Set up CI/CD pipeline with GitHub Actions
- Add dark/light theme toggle
- Implement more interactive project showcases

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

- Email: tharunk1915@gmail.com
- LinkedIn: [Tharun K](https://www.linkedin.com/in/tharun-k-18b8b2262)
- GitHub: [Tharun19102002](https://github.com/Tharun19102002)