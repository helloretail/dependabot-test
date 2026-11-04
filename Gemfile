source "https://rubygems.org"

# Bundle edge Rails instead: gem "rails", github: "rails/rails", branch: "main"
gem "rails", "~> 8.0.4"
# The modern asset pipeline for Rails [https://github.com/rails/propshaft]
gem "propshaft"
# Use postgresql as the database for Active Record
gem "pg", "~> 1.1"
# Use the Puma web server [https://github.com/puma/puma]
gem "puma", ">= 5.0"
# Use JavaScript with ESM import maps [https://github.com/rails/importmap-rails]
gem "importmap-rails"
# Hotwire's SPA-like page accelerator [https://turbo.hotwired.dev]
gem "turbo-rails"
# Hotwire's modest JavaScript framework [https://stimulus.hotwired.dev]
gem "stimulus-rails"
# Use Tailwind CSS [https://github.com/rails/tailwindcss-rails]
gem "tailwindcss-rails"

# Use Active Model has_secure_password [https://guides.rubyonrails.org/active_model_basics.html#securepassword]
gem "bcrypt", "~> 3.1.7"

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem "tzinfo-data", platforms: %i[ windows jruby ]

# Use the database-backed adapters for Rails.cache, Active Job, and Action Cable
gem "solid_cache"
gem "solid_queue"
gem "solid_cable"

# Reduces boot times through caching; required in config/boot.rb
gem "bootsnap", require: false

# Deploy this application anywhere as a Docker container [https://kamal-deploy.org]
gem "kamal", require: false

# Add HTTP asset caching/compression and X-Sendfile acceleration to Puma [https://github.com/basecamp/thruster/]
gem "thruster", require: false

# HTTP client for Pipedrive API
gem "faraday"
# Official Model Context Protocol SDK — powers the read-only Pipedrive MCP
# endpoint at /mcp/:token (see app/controllers/mcp_controller.rb).
gem "mcp"
# OpenAI API client
gem "ruby-openai"
# Google Sheets ingestion (cancellation events from the finance master
# sheets): service-account Drive export + XLSX parsing
gem "google-apis-drive_v3"
gem "googleauth"
gem "roo", "~> 2.10"
# WHOIS lookups for domain verification
gem "whois", "~> 6.0"
gem "whois-parser"
# Registrable domain (eTLD+1) computation — handles .co.uk / .com.au correctly
gem "public_suffix", "~> 5.1"
# Phone number parsing/validation backed by Google libphonenumber data —
# handles "0039…" international prefix, national-format "0…", per-country
# format/length validation, and E.164 formatting.
gem "phonelib", "~> 0.10"
# QR code generation (display pairing flow)
gem "rqrcode", "~> 3.2"
# Faraday redirect following (extracted from Faraday 2.x)
gem "faraday-follow_redirects"
# Headless Chrome for JavaScript-rendered page inspection (enrichment crawlers)
gem "ferrum"
# Thread-safe concurrency primitives for parallel Scrapfly fetching
gem "concurrent-ruby"
# Fast HTML parser based on Lexbor — 5x faster than Nokogiri, thread-safe architecture
gem "nokolexbor"
# ZIP file extraction (Wappalyzer delivers lead lists as ZIP/CSV)
gem "rubyzip", "~> 2.3", require: "zip"
# CSV parsing (CSV Domain Checker upload). Declared explicitly because csv leaves
# Ruby's default gems in 3.4; without this it warns on every load under 3.3.
gem "csv"
# Throttling middleware for public endpoints
gem "rack-attack"
# Bound request duration so a slow upstream (Pipedrive, OpenAI, Scrapfly) can't
# pin a Puma thread indefinitely and starve health checks. Configured via
# RACK_TIMEOUT_SERVICE_TIMEOUT / RACK_TIMEOUT_WAIT_TIMEOUT env vars.
gem "rack-timeout"
# AWS S3 backend for ActiveStorage (Hello Scout build ZIPs)
gem "aws-sdk-s3", require: false

group :development, :test do
  gem "debug", platforms: %i[ mri windows ], require: "debug/prelude"
  gem "brakeman", require: false
  gem "rubocop-rails-omakase", require: false
  gem "rspec-rails"
  gem "factory_bot_rails"
  gem "webmock"
  gem "dotenv-rails"
  gem "climate_control"
  gem "capybara"
end

group :development do
  gem "web-console"
end

gem "neighbor", "~> 0.6.0"

gem "jwt", "~> 3.2"

gem "holidays", "~> 8.8"
