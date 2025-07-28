# 🌐 Agnostic/holistic API Naming & Structure Guidelines

> _"A clear and adaptable approach to naming, structuring, and sharing API collections in Postman for better collaboration and long-term maintainability.”_

---

## 🎯 Purpose

This guide aims to establish a clear, scalable, and easy-to-maintain naming convention and structural approach for API requests in Postman. It is designed to help cross-functional teams collaborate smoothly while maintaining consistency and quality in rapidly evolving projects.

---

## 📛 Request Naming Convention

**Recommended format:**

[HTTP Method] Clear Action | Module or Client

### 🧪 Examples

- `GET Fetch users | Admin`
- `POST Create payment | Bank Agricola`
- `DELETE Remove account | Customer`
- `PUT Update password | Security`
- `GET Session status | Auth`
- `POST Login | Dummy Auth`

💡 The pipe symbol `|` visually separates the action from its context and improves scan-ability.

---

## 🗂️ Folder Structure

Folders should represent **functional modules, teams, or services**.

Example:

tn-api-branching-demo/
├── Ra (Core/Auth)
│ └── GET Session status | Auth
│ └── POST Login | Dummy
├── Thoth (Reports)
│ └── GET Fetch analytics | JSONPlaceholder
├── Bastet (Users)
│ └── GET Fetch users | ReqRes
├── Osiris (External Integrations)
│ └── GET External config | httpbin

---

## 🧠 Additional Best Practices

- ✅ Include a clear **description** in each request (purpose, parameters, headers).
- ✅ Use **consistent and descriptive names**.
- ✅ Avoid internal-only acronyms unless documented.
- ✅ Use environment variables (`{{baseUrl}}`, `{{authToken}}`) instead of hardcoding values.
- ✅ Document the **auth mechanism** (Bearer, Basic, API Key) if required.
- ✅ Include **basic tests** in Postman to validate responses and status codes.

---

## 🤝 Team Culture & Evolution

This guide is a living document. As the API evolves and the team grows, feel free to suggest improvements and keep this guide up to date. The goal is not rigidity, but clarity with purpose. 💫

---

## 📚 References

- [Postman Learning Center – Naming Requests & Structuring Collections](https://learning.postman.com/docs/publishing-your-api/naming-guidelines/)
- [OpenAPI Initiative – API Design Guidelines](https://spec.openapis.org/oas/latest.html)
- [Google API Design Guide](https://cloud.google.com/apis/design)
- [Microsoft REST API Guidelines](https://github.com/microsoft/api-guidelines)
- [Stripe API Reference – Example of consistent and clean naming](https://stripe.com/docs/api)

---

Made with ❤️ by Onofre Liscano — Helping build clean APIs, one request at a time.
