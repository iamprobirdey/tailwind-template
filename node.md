# How to install tailwind css using postcss

# Command to follow:

# npm init -y
# npm install -D tailwindcss postcss-cli autoprefixer
# npx tailwindcss init -p

# config of postcss.config.js 

# module.exports = {
#  plugins: {
#    tailwindcss: {},
#    autoprefixer: {},
#  }
# }

# config of tailwind.config.js

# module.exports = {
#  content: ["./src/**/*.{html,js}"],
#  theme: {
#    extend: {},
#  },
#  plugins: [],
# }

# config of style.css

# @tailwind base;
# @tailwind components;
# @tailwind utilities;


# config of package.json

#  "dev": "TAILWIND_MODE=WATCH postcss tailwind.css -o output/css/style.css --watch --verbose",
#    "prod": "NODE_ENV=production postcss tailwindcss -o output/css/style.css "