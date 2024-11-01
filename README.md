# Walmart Data Scraping Project

This project successfully scrapes comprehensive product data from [Walmart.com](https://www.walmart.com/), overcoming multiple security challenges to provide structured data in JSON format. You’ll find a sample dataset included for reference.

## Project Overview

- **Website**: Walmart.com
- **Goal**: Full data extraction, including product information, pricing, reviews, availability, and more.
- **Challenges Encountered**:
  - **IP Blocking**
  - **Press & Hold Captcha**
  - **Security Layers**: PerimeterX and Akamai Bot Manager

## Solution Approach

To tackle the website's IP blocking and captcha challenges, advanced bypassing techniques were employed. These include:
- **IP Rotation**: Randomly changing IP addresses to avoid detection.
- **Custom Headers and User-Agents**: Mimicking regular web traffic patterns to reduce bot suspicion.
- **Captcha Bypass**: Successfully managed Press & Hold captchas by manipulating IPs and headers.

## Data Fields

The scraped data covers various fields to provide complete product details, including but not limited to:

- **ProductId**: Unique identifier for each product
- **ProductUrl**: Direct link to the product on Walmart
- **ProductName**: Name of the product
- **Category**: Product category
- **ProductPrice**: Current price
- **AvailabilityStatus**: Stock information
- **Rating and Reviews**: Customer feedback
- **ReturnPolicy**: Return options and conditions
- **ProductImages**: Array of image URLs
- **ProductDescription**: Detailed description of the product

## Sample Data

Here's a sample of the extracted data:

```json
{
    "ProductId": "2UW4JTE2A5UZ",
    "ProductUrl": "https://www.walmart.com/ip/Men-s-1-10-ctw-Black-Diamond-Black-Tungsten-Grooved-8MM-Wedding-Band-Men-s-Ring/949552322?classType=VARIANT",
    "ProductName": "Brilliance Fine Jewelry Men's 1/10 Ctw Black Diamond Black Tungsten Grooved 8MM Wedding Band - Men's Ring",
    "category": "Jewelry",
    "ProductPrice": "$98",
    "availabilityStatus": "In stock",
    "rating": 4.4,
    "numberOfReviews": 112,
    "brand": "Brilliance Fine Jewelry",
    "returnPolicy": {
        "returnable": true,
        "freeReturns": true,
        "returnWindow": {
            "value": 90,
            "unitType": "Day"
        },
        "returnPolicyText": "Free Holiday returns until Jan 31"
    },
    "description": "Bold and elegant black diamonds make a striking statement...",
    "ProductImages": [
        {"url": "https://i5.walmartimages.com/seo/Men-s-1-10-ctw-Black-Diamond-..."}
    ],
    "reviews": {
        "customerReviews": [
            {
                "reviewId": "360058301",
                "rating": 5,
                "reviewText": "This ring is amazing quality for the price...",
                "userNickname": "Sav",
                "features": [{"name": "Ring size", "value": "7"}]
            }
        ],
        "topNegativeReview": {
            "reviewId": "359851258",
            "rating": 2,
            "reviewText": "I had this as a gift to my husband..."
        }
    }
}
```



## Sample Data

For a quick overview of the scraped data structure, refer to the sample files in this repository:

- `walmart.com_sample_data.json`

These files illustrate the kind of information collected from RealSelf, making it easier to analyze and utilize the data.

## Contact Me

For any inquiries or service requests, please reach out to me via LinkedIn or visit my portfolio website:

- **LinkedIn**: [Mominur Rahman](https://www.linkedin.com/in/mominur--rahman/)
- **Portfolio Website**: [mominur.dev](https://mominur.dev)
- **Blog Posts**: [Mominur's Blog](https://mominur.dev/posts.html)

I look forward to connecting with you!
