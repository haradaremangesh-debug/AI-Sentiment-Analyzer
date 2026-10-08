# Sentiment Analyzer v2

A lightweight, browser-based sentiment analyzer built with **HTML, CSS, and JavaScript**.

## Features

- Positive, negative, and neutral sentiment classification
- Character counter with a 1500-character limit
- Example sentences for positive, negative, and neutral sentiment
- Sentiment strength progress bar
- Positive/negative word detection
- Basic booster-word handling (`very`, `really`, `extremely`, etc.)
- Basic negation handling (`not`, `never`, `don't`, etc.)
- Responsive design for desktop and mobile
- No login, signup, database, server, or external API required

## Files

- `sentiment_analyzer_v2.html` — complete source code for the application.
- `README.md` — project documentation.

## How It Works

The application uses a client-side JavaScript word-list approach rather than a machine-learning model or external AI API.

1. The user enters text.
2. The text is converted to lowercase and tokenized.
3. Words are compared against positive and negative word lists.
4. Booster words increase the effect of the following sentiment word.
5. Negation words reverse the effect of nearby sentiment words.
6. The resulting score determines `POSITIVE`, `NEGATIVE`, or `NEUTRAL`.
7. A sentiment-strength percentage is displayed.

## How to Run

No installation is required.

1. Keep `sentiment_analyzer_v2.html` and `README.md` in the same folder.
2. Double-click `sentiment_analyzer_v2.html`, or open it in any modern web browser.
3. Enter a sentence or paragraph.
4. Click **Analyze Sentiment**.

## Important Notes

This is a rule-based sentiment analyzer. It is described in the UI as “AI-style” classification, but it does not call an AI model or machine-learning service.

The analyzer works primarily with the English words included in its built-in positive and negative word lists. It may therefore produce inaccurate results for sarcasm, complex context, unfamiliar vocabulary, or languages other than English.

## Customization

You can customize the sentiment vocabulary directly in the JavaScript section:

- `pos` — positive words
- `neg` — negative words
- `boost` — words that strengthen sentiment
- `negator` — words that reverse nearby sentiment

You can also modify the CSS variables at the top of the stylesheet to change the application's colors and visual style.

## Technology

- HTML5
- CSS3
- Vanilla JavaScript
- No external dependencies

## License

No license is specified in the supplied source file. Add a license if you plan to distribute the project publicly.
