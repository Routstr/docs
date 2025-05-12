# Routstr Documentation

This repository contains the official documentation for Routstr, a decentralized LLM routing marketplace powered by Nostr and Bitcoin.

## About Routstr

Routstr brings the convenience of centralized AI providers to the permissionless, censorship-resistant world of Nostr and Bitcoin. It enables seamless access to AI models through an OpenAI-compatible API while maintaining privacy, reducing costs, and eliminating traditional payment barriers.

### Core Features

- **OpenAI-Compatible API**: Easy integration with existing tools and libraries that support the OpenAI API format
- **Self-Hosted Proxy**: Turn any OpenAI-compatible endpoint into a pay-as-you-go business without Stripe or KYC requirements
- **Privacy Routing**: Built-in SOCKS5 and Tor support for enhanced privacy and censorship resistance
- **Decentralized Payments**: Cashu ecash tokens and Lightning payments for prepaid, private transactions

## Getting Started

### For Users

Access AI models through Routstr by:

1. Obtaining Cashu tokens with Lightning or on-chain Bitcoin
2. Using the token in API requests to `https://api.routstr.com/v1/chat/completions`
3. Making requests with your preferred OpenAI-compatible client library

### For Providers

Set up your own Routstr node to offer AI models:

1. Deploy the Routstr proxy in front of your OpenAI-compatible API endpoint
2. Configure payments via Cashu or Lightning
3. Set custom pricing for different models
4. Announce your service to the Routstr network via Nostr

## Documentation Development

This documentation is built with Mintlify. To preview changes locally:

### Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview the documentation changes locally:

```
npm i -g mintlify
```

Run the following command at the root of the documentation:

```
mintlify dev
```

### Publishing Changes

Changes will be deployed to production automatically after pushing to the default branch.

### Repository Structure

The Routstr project consists of several key repositories:

- [protocol](https://github.com/routstr/protocol): Technical specification and improvement protocol
- [frontend](https://github.com/routstr/frontend): The main public facing website
- [proxy](https://github.com/routstr/proxy): Running in front of any OpenAI-compatible API to handle API key payments
- [evals](https://github.com/routstr/evals): Quality control for language model endpoints
- [docs](https://github.com/routstr/docs): This documentation repository

## Additional Resources

- Website: [https://routstr.com](https://routstr.com)
- API Documentation: [https://api.routstr.com/docs](https://api.routstr.com/docs)
- GitHub: [https://github.com/routstr](https://github.com/routstr)
- Contact: [team@routstr.com](mailto:team@routstr.com)
