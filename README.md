Foodpanda Clone (Pure HTML & CSS Architecture)
Educational & Learning Showcase: A fully interactive multi-page frontend clone of foodpanda built strictly with HTML5 and modern CSS3 (Tailwind utility integration), featuring zero JavaScript.
Educational Disclaimer
This project is created strictly for educational, portfolio, and learning purposes.
All registered trademarks, logos, brand names, and service concepts (such as foodpanda, pandamart, and Pau-Pau) belong to Foodpanda / Delivery Hero SE.
This repository is not affiliated with, endorsed by, or sponsored by Delivery Hero or Foodpanda in any capacity.
No commercial transactions, data collection, or real monetary checkouts take place within this project.
Architecture: 5 Pages Across 3 Connected Layers
The core objective of this project is demonstrating how to build a deep, sequential user pipeline using a pure CSS routing engine (hidden radio inputs paired with <label for="..."> activations):
┌────────────────────────────────────────────────────────┐
│  LAYER 1: Discovery & Entry Hubs                       │
│  ├── Page 1: Home Delivery Landing Hub (#page-1)       │
│  └── Page 2: Pandamart 15-Minute Grocery Hub (#page-2) │
└──────────────────────────┬─────────────────────────────┘
                           │ (Clicking category or search)
                           ▼
┌────────────────────────────────────────────────────────┐
│  LAYER 2: Catalog & Browse Hubs                        │
│  ├── Page 3: Restaurant Listings & Directory (#page-3) │
│  └── Page 4: Daily Mega Deals & Vouchers Hub (#page-4) │
└──────────────────────────┬─────────────────────────────┘
                           │ (Selecting a restaurant or voucher)
                           ▼
┌────────────────────────────────────────────────────────┐
│  LAYER 3: Fulfillment & Action                         │
│  └── Page 5: Restaurant Menu, Basket Drawer &          │
│              Live GPS Tracker (#page-5)                │
└────────────────────────────────────────────────────────┘


1. Layer 1: Entry & Discovery Hubs
Page 1 (Home Landing): Hero banner, location indicator, fast-access category cards (Food Delivery, Pandamart, Deals, Pick-up), popular cuisine pills, and featured spot previews.
Page 2 (Pandamart Grocery Store): Quick-commerce shelf view with categorized items (dairy, fresh produce, cold drinks, snacks) and 15-minute fulfillment stats.
2. Layer 2: Catalog & Deals Hubs
Page 3 (Restaurant Listings): Multi-attribute listing view showing meal categories, ratings, delivery times, and fee indicators.
Page 4 (Mega Deals & Vouchers): Promo vouchers (PANDA50, FREEDEL, MART200) and bundle savings with direct links into checkout.
3. Layer 3: Action & Fulfillment
Page 5 (Restaurant Menu, Basket & GPS): Specific restaurant showcase, food menu catalog, live delivery tracker simulation, and a pure CSS slide-out cart drawer with pricing breakdown and voucher calculation.
🛠️ Technical Highlights & Techniques
Feature
How It's Implemented
Zero JavaScript Routing
Sibling selector technique: #page-X:checked ~ main #page-view-X toggles active screen visibility.
Interactive Transitions
HTML <label for="page-X"> elements serve as declarative, accessible click targets.
Pure CSS Cart Drawer
Checkbox toggle trick (#cart-toggle:checked ~ #cart-modal) with CSS keyframe sliding animation.
Responsive Grid & Flexbox
Tailwind CSS utility classes ensure mobile-first responsiveness across phones, tablets, and desktops.
Design Consistency
Replicates Foodpanda's signature brand pink (#d70f64), soft pink card accents (#fdf2f6), and bold typography.

📂 Project Structure
foodpanda-clone/
├── index.html        # Semantic HTML5 markup containing all 5 page views and modal layers
├── styles.css        # CSS routing engine, pseudo-states, modal animations, and scrollbars
└── README.md         # Documentation & architectural overview


🚀 How to Run Locally
Because this project requires no build tools, bundlers, or JavaScript dependencies, you can run it instantly:
Clone or download this repository:
git clone https://github.com/your-username/foodpanda-clone.git
cd foodpanda-clone


Ensure both index.html and styles.css are in the same folder.
Open index.html directly in your favorite web browser (Chrome, Firefox, Safari, Edge):
# On macOS
open index.html

# On Windows
start index.html

# On Linux
xdg-open index.html


🎓 Learning Takeaways
Building complex, single-page application (SPA) user flows using purely native web standards.
Deepening mastery of CSS state management (:checked, :focus-within, sibling combinators ~ and +).
UI/UX structuring for multi-tiered e-commerce platforms (Discovery  Catalog  Checkout).
