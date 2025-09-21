Pricing Card Component

This project refactors a broken pricing card snippet into a reusable component using HTML, CSS, and JavaScript.

📌 Before (Broken Snippet)

Issues with the original code:

box-shdow typo (should be box-shadow)

Unclosed <h2> tag

Buttons were unresponsive

Not reusable (hardcoded content)

✅ After (Refactored & Reusable)

The card is now:

Responsive and styled with clean CSS

Fixed HTML errors

Encapsulated in a reusable function:

createPricingCard({ title, price, features, buttonText })


You can now generate multiple cards with different values (Basic, Pro, Enterprise, etc.).

🚀 How to Use

Clone the repo and open index.html in your browser.

The reusable function is inside a <script> tag:

document.getElementById("pricing-container").innerHTML = createPricingCard({
  title: "Basic Plan",
  price: "$9.99 / month",
  features: ["1 GB Storage", "Basic Support", "All Core Features"],
  buttonText: "Start Trial"
});


Add more plans by calling createPricingCard() again with different arguments.

🤖 AI Prompt Used in Cursor

Here’s the exact prompt used to fix and refactor the snippet:

"Here’s a broken pricing card layout. Please fix the layout bugs (e.g., unclosed tags, CSS typos), make the button responsive, and refactor it into a reusable function createPricingCard({ title, price, features, buttonText }) that I can call with different values. Keep the styling clean and modern. Here’s the broken snippet: [paste original code]"
