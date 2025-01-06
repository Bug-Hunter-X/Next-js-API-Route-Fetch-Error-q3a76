# Next.js API Route Fetch Error

This repository demonstrates a common error encountered when using custom API routes in Next.js applications to make external API requests. The issue involves a `TypeError: Failed to fetch` error, often stemming from CORS (Cross-Origin Resource Sharing) restrictions.

## Bug

The `pages/api/data.js` file attempts to fetch data from an external API. Due to CORS policies, this request may fail unless the external API is configured to allow requests from your Next.js application's domain.

## Solution

The solution involves either configuring the external API to allow CORS requests from your Next.js application or using a proxy server to handle the API request.

The `pages/api/data.js` file is updated with a proxy setting to get around CORS issues and successfully fetch the data.