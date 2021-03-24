# [Justdial Scraper](https://nileshkant.github.io/justdial-website-scrapper/)

![alt text][logo]

[logo]: https://i.imgur.com/IZAwGLg.jpg 'Justdial data extractor'

An automation script written in Node.js, powered by Puppeteer to scrap multiple pages of Justdial (an Indian Yellow Pages website) and exports specific information in JSON format.

> **Disclaimer**  
> It is illegal to scrape JustDial, but the code is made open-source purely for educational purposes to understand technologies like NodeJS, Puppeteer and Automation Testing.

It will extract data of specific business query from a city, from justdial in Json form given below.

---

## Example

---

```yaml
 {
    "name": "Sagar Clinic and Day Care",
    "url": "https://www.justdial.com/Bangalore/Sagar-Clinic-and-Day-Care-Near-Petrol-Bunk-Jp-Nagar-7th-Phase/080PXX80-XX80-190215112653-J9Y1_BZDET?xid=QmFuZ2Fsb3JlIERvY3RvcnM=",
    "phoneNumber": "+(91)-080-41710009",
    "rating": "4.6",
    "votes": "27",
    "address": "No 47/26/27, 12th Main, Puttenhalli Main Road, Jp Nagar 7th Phase, Bangalore - 560078, Near Petrol Bunk",
    "categories": "General Physician Doctors, Home Nursing Services",
    "businfo": "Sagar Clinic and Day Care in Jp Nagar 7th Phase, Bangalore\n\nSagar Clinic and Day Care in Bangalore is one of the leading businesses in the Physiotherapists For Joint Pain."
    "faq": "1. What are the various mode of payment accepted here ?\n\nYou can make payment Via Cash, Master Card, Credit Card.\n\n2. Which is the nearest landmark ?\n\nYou can easily locate the establishment as it is in close proximity to Near Petrol Bunk"
  }
```

## Installation

```sh
$ npm install
```

## Usage

Change these values in line 6-9 of `index.js`:

```javascript
const CITY = 'Mumbai';
const KEYWORD = 'street-foods';
const INITIAL_PAGE = 0;
const NUMBER_OF_PAGES = 2;
```

```sh
$ npm start
```
