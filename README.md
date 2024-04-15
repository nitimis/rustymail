# RustyMail

RustyMail is a fully open-source, asynchronous email server solution designed to handle both inbound and outbound emails efficiently. Built with Rust and leveraging modern asynchronous programming models, it ensures high performance and scalability. It supports SMTP for sending emails and IMAP for receiving, with plans to extend functionality in future releases.

## Features

* SMTP Support: Send emails using the Simple Mail Transfer Protocol.
* IMAP Support: Receive emails using the Internet Message Access Protocol.
* Queue Management: Robust handling of email queues to manage workload and priorities.
* Bounce Handling: Automatic handling of bounced emails to maintain sender reputation.
* Security: Implements TLS to ensure secure email transmission.
* Scalability: Designed to scale horizontally on Kubernetes platforms.
* Docker Support: Containerized deployment for ease of installation and maintenance.

## Getting Started

### Prerequisites

* Rust
* SurrealDB

### Configuration

* SMTP and IMAP settings: Edit the config.toml file to adjust the SMTP and IMAP server settings according to your needs.
* Database: Configure SurrealDB connection strings within the config.toml.

# Example command to send an email

cargo run --bin rustymail-cli -- send --from sender@example.com --to receiver@example.com --subject "Test Email" --body "Hello, this is a test email from AsyncRustMail."

Contributing

We welcome contributions from the community, whether it's adding new features, improving documentation, or reporting bugs. Please refer to [CONTRIBUTING.md](CONTRIBUTING.md) for more details on how to contribute.

Roadmap

* SMTP and IMAP implementation
* Email tracking and analytics
* Advanced filtering and spam detection

License

This project is dual-licensed under the MIT License & Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details.
