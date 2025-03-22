# Walmart Data Scraping Project

This project successfully scrapes comprehensive product data from [Walmart.com](https://www.walmart.com/), overcoming multiple security challenges to provide structured data in JSON format. You’ll find a sample dataset included for reference.

# ⚠️ **Important Notice: Business Use Only** ⚠️

This repository is for **demonstration purposes only** and **not for free use**. It showcases my professional expertise in **web scraping** and **automation**.

🚫 **Unauthorized use, redistribution, or modification is strictly prohibited.**

💼 **For custom web scraping and automation solutions, please contact me directly for professional, business-focused services.**

📩 [Get in Touch](https://mominur.dev)

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
    "wasPrice": "",
    "savingsAmount": "",
    "sellerName": "Walmart.com",
    "availabilityStatus": "In stock",
    "rating": 4.4,
    "numberOfReviews": 112,
    "brand": "Brilliance Fine Jewelry",
    "manufacturerProductId": "TG17204",
    "returnPolicy": {
        "returnable": true,
        "freeReturns": true,
        "returnWindow": {
            "value": 90,
            "unitType": "Day"
        },
        "returnPolicyText": "Free Holiday returns until Jan 31",
        "returnPolicyTextCode": {
            "code": "PRODUCT_HOLIDAY_RETURN",
            "data": null
        },
        "returnPolicyCondition": null,
        "holidayReturnEnabled": true
    },
    "description": "Bold and elegant black diamonds make a striking statement in this black ion-plated tungsten men's wedding ring. Step away from traditional wedding band choices and select a unique ring that truly reflects your style and personality.  This modern design is perfect for men of all ages\u2014whether you\u2019re a teenager looking to make your mark, a young adult ready to commit, or a senior celebrating a lifetime of love. The eye-catching black diamonds are complemented by the sleek tungsten band, creating a distinctive look that stands out on any occasion.  Embrace your individuality with this stylish black ion-plated tungsten ring, a perfect choice for anyone seeking a contemporary and sophisticated wedding band.",
    "ProductImages": [
        {
            "url": "https://i5.walmartimages.com/seo/Men-s-1-10-ctw-Black-Diamond-Black-Tungsten-Grooved-8MM-Wedding-Band-Men-s-Ring_1b8b58e3-3119-4020-a8c1-1bcc4a8c7da0.c487b34ddd2267ec0018e877b2308a83.jpeg"
        },
        {
            "url": "https://i5.walmartimages.com/asr/10fe3fca-a156-43de-8071-6172d3420909.9764ef731c98a7230689f8ead754e6c2.jpeg"
        },
        {
            "url": "https://i5.walmartimages.com/asr/0cd08853-3632-4c78-8953-2f0c0d6a4223.18f699126bb6fc945be679dcd56dc442.jpeg"
        },
        {
            "url": "https://i5.walmartimages.com/asr/4c26bec3-7742-44fa-8d47-88672992c112.2d9efab43a6c248b0d6f5ae8be6a5197.jpeg"
        }
    ],
    "reviews": {
        "customerReviews": [
            {
                "reviewId": "360058301",
                "rating": 5,
                "reviewSubmissionTime": "10/12/2024",
                "reviewText": "This ring is amazing quality for the price. My husband loves it. He never takes it off and it looks the same way it did when I purchased it.",
                "reviewTitle": "Great quality!",
                "negativeFeedback": 0,
                "positiveFeedback": 0,
                "userNickname": "Sav",
                "fulfilledBy": "Walmart",
                "status": null,
                "sellerName": "Walmart.com",
                "media": null,
                "photos": [],
                "badges": [
                    {
                        "badgeType": "Custom",
                        "id": "VerifiedPurchaser",
                        "contentType": "REVIEW",
                        "glassBadge": {
                            "id": "VerifiedPurchaser",
                            "text": "Verified Purchase"
                        }
                    }
                ],
                "clientResponses": null,
                "syndicationSource": null,
                "snippetFromTitle": null,
                "features": [
                    {
                        "name": "Ring size",
                        "value": "7"
                    }
                ]
            }
        ],
        "topNegativeReview": {
            "reviewId": "359851258",
            "rating": 2,
            "reviewSubmissionTime": "10/10/2024",
            "userNickname": "Laura",
            "negativeFeedback": 0,
            "positiveFeedback": 0,
            "reviewText": "I had this as a gift to my husband. I wrote a special note to come with it and they didn't put it in there so it ruined my vow renewal question ring is perfect but ruined everything that was planned.",
            "reviewTitle": null,
            "badges": [
                {
                    "badgeType": "Custom",
                    "id": "VerifiedPurchaser",
                    "contentType": "REVIEW",
                    "glassBadge": {
                        "id": "VerifiedPurchaser",
                        "text": "Verified Purchase"
                    }
                }
            ],
            "clientResponses": null,
            "syndicationSource": null,
            "snippetFromTitle": null,
            "media": null
        },
        "topPositiveReview": {
            "reviewId": "360058301",
            "rating": 5,
            "reviewSubmissionTime": "10/12/2024",
            "userNickname": "Sav",
            "negativeFeedback": 0,
            "positiveFeedback": 0,
            "reviewText": "This ring is amazing quality for the price. My husband loves it. He never takes it off and it looks the same way it did when I purchased it.",
            "reviewTitle": "Great quality!",
            "badges": [
                {
                    "badgeType": "Custom",
                    "id": "VerifiedPurchaser",
                    "contentType": "REVIEW",
                    "glassBadge": {
                        "id": "VerifiedPurchaser",
                        "text": "Verified Purchase"
                    }
                }
            ],
            "syndicationSource": null,
            "snippetFromTitle": null,
            "clientResponses": null,
            "media": null
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

- **Portfolio:** [mominur.dev](https://mominur.dev)
- **GitHub:** [github.com/mominurr](https://github.com/mominurr)
- **LinkedIn:** [linkedin.com/in/mominur--rahman](https://www.linkedin.com/in/mominur--rahman/)
- **Email:** mominurr518@gmail.com

I look forward to connecting with you!
