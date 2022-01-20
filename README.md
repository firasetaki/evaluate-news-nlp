# Evaluate a text with Natural Language Processing

## About the Project

This is the 4th project of the [Udacity Front End Web Developer Nanodegree program](https://www.udacity.com/course/front-end-web-developer-nanodegree--nd0011).

The project aims to build a web tool that uses Natural Language Processing (NLP) techniques to perform sentiment analysis of a text from different sources on the internet. The analysis is provided by [MeaningCloud](https://learn.meaningcloud.com/developer/sentiment-analysis/2.1/doc/what-is-sentiment-analysis).

### Analysis Scope

The analysis performed on the text identifies the following sentiments:

- Polarity: Indicates the global polarity of the text
- Agreement: Marks the agreement between the sentiments detected in the text
- Confidence: Represents the confidence associated with the sentiment analysis performed on the text
- Subjectivity: Marks the subjectivity of the text
- Irony: Indicates the irony of the text.

### Built with

- Front-end: HTML, SASS and JavaScript
- Back-end: Node and ExpressJS
- Build tool: Webpack
- PWA: Workbox
- Testing: Jest

### Functionality

- Call an api from the server-side on form submission
- Update the User Interface dynamically to log the latest information from the api response
- Implement an offline functionality using Workbox
- Apply unit tests using Jest
- Apply simple form validation and return an error to alert the user when the input is empty or the provided URL is not valid.

## Getting Started

### Prerequisites

Make sure Node and NPM are installed on your computer. Otherwise, install both.

1. Node: Binaries, installers, and source tarballs are available at <https://nodejs.org/en/download/>.

2. NPM: From the terminal
   ```sh
   npm install npm -g
   ```

### Installation

1. Get a free API Key at [MeaningCloud](https://www.meaningcloud.com/)

2. Clone the project repo

   ```sh
   git clone https://github.com/firagoras/evaluate-news-nlp.git
   ```

3. Install NPM packages

   ```sh
   npm install
   ```

4. Configure environment variables using dotenv package

- Create a new `.env` file in the root of your project

- Fill the `.env` file with your API key like this:
  ```js
  const API_KEY = 'ENTER YOUR API';
  ```

5. Start the project front-end

- Run on development mode
  ```sh
  npm run build-dev
  ```
- Run on production mode
  ```sh
  npm run build-prod
  ```

6. Run the server

   ```sh
   npm run start
   ```

### Testing

- Unit test
  ```sh
  npm run test
  ```

## Usage

Submit the URL of a text and click "Analyse", the page displays the analysis results as returned form the MeaningCloud Sentiment Analysis API
