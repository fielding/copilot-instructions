# Copilot Code Generation Instructions

[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](CONTRIBUTING.md)
[![CC BY 4.0][cc-by-shield]][cc-by]

[cc-by]: https://creativecommons.org/licenses/by/4.0/
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg


A community-driven collection of code generation instructions for GitHub Copilot's experimental feature. Customize Copilot to follow your preferred coding styles, frameworks, and best practices!

---

## 🚀 **Introduction**

GitHub Copilot has introduced an experimental feature that allows developers to provide **Code Generation Instructions**. These instructions guide Copilot to generate code that adheres to your specific coding styles, uses preferred libraries, and follows best practices.

This repository serves as a centralized collection of such instructions, categorized by programming languages and frameworks. Whether you're using Python, JavaScript, or any other language, you'll find tailored instructions to enhance your Copilot experience.

*note*: The instruction sets provided here are intended as starting points. We understand that no single set of instructions will be perfect for everyone, and that's perfectly fine. Our primary goal is to raise awareness of this GitHub Copilot feature and offer initial versions for you to customize and build upon according to your needs. We encourage you to contribute your own suggestions and improvements to help enhance this resource for everyone!

---

## 🎯 **What Are Code Generation Instructions?**

Code Generation Instructions are guidelines that you can provide to GitHub Copilot to influence the code it generates. They can specify:

- Coding styles and conventions
- Preferred libraries and frameworks
- Commenting and documentation styles
- Design patterns and architectural principles

By setting these instructions, Copilot can produce code that better fits your project's needs and your personal or team's coding standards.

---

## 🛠 **How to Use Code Generation Instructions**

1. **Enable the Experimental Feature:**

   Ensure you have the latest version of GitHub Copilot and that the experimental feature `github.copilot.chat.experimental.codeGeneration.instructions` is enabled in your VS Code settings.

2. **Select Instruction Files:**

   - Browse the `/instructions/` directory in this repository to find instruction files that suit your needs.
   - Instruction files are organized by programming language and framework.
   - Feel free to customize these instruction files by adding, modifying, or removing instructions to fit your specific requirements.

3. **Combine Instruction Files (Optional):**

   You can combine multiple instruction files to tailor Copilot's code generation to your preferences.

   **Example:**

   To combine the base Python instructions with NumPy-specific instructions:

   ```bash
   cd instructions/python
   cat base.md numpy.md > ../../.vscode/copilot-instructions.md
   ```

4. **Add Instructions to Your Project:**

   Place the combined instruction file at `.vscode/copilot-instructions.md` in the root directory of your project.

5. **Update Your VS Code Settings:**

   Add the following configuration to your `settings.json` file:

   ```json
   "github.copilot.chat.experimental.codeGeneration.instructions": [
     {
       "file": ".vscode/copilot-instructions.md"
     }
   ],
   ```

6. **Restart VS Code:**

   Reload or restart VS Code to apply the new settings.

---

## 🌟 **Features of This Repository**

- **Community Contributions:** A growing collection of instruction sets contributed by developers worldwide.
- **Organized Structure:** Instructions are categorized by language and framework for easy navigation.
- **Customizable:** Combine and modify instruction files to suit your coding style and project requirements.
- **Open to Feedback:** We're eager to collaborate with the community to refine and improve these instructions.

---

## 📂 **Repository Structure**

```
copilot-instructions/
├── README.md
├── CONTRIBUTING.md
├── LICENSE
├── CODE_OF_CONDUCT.md
└── instructions/
    ├── python/
    │   ├── base.md
    │   ├── numpy.md
    │   ├── pandas.md
    │   └── README.md
    ├── javascript/
    │   ├── base.md
    │   ├── react.md
    │   └── README.md
    └── [other languages]/
        ├── [instruction files].md
        └── README.md
```

---

## 🛠 **Customization**

These instruction files are general guidelines. We encourage you to customize them to suit your specific needs. Feel free to add, modify, or remove instructions based on your coding style preferences and project requirements.

It's worth noting that the purpose of this feature is to guide Copilot in generating code that aligns with *your* standards. It's ultimately about your style and preferences, so please make sure to customize these instructions accordingly.

---

## 🤝 Contributing

We welcome contributions! Please read our [Contributing Guidelines](CONTRIBUTING.md) and adhere to our [Code of Conduct](CODE_OF_CONDUCT.md).

---

## 💡 **Community Standards**

We are open to feedback and collaboration to define and refine community standards for Copilot code generation instructions. The decisions made here are just a starting point, and we welcome your input to make this resource better for everyone.

---

## 📜 License

This work is licensed under the [Creative Commons Attribution 4.0 International License](LICENSE).



---

## 📧 **Contact**

For questions, suggestions, or feedback, feel free to open an issue or reach out via email at [fielding@justfielding.com](mailto:fielding@justfielding.com).

---

## ⭐ **Acknowledgments**

Shoutout to the GitHub Copilot team for introducing this experimental feature and empowering developers to customize their code generation experience!

---

## 🔗 **Links**

- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [VS Code August Update (1.93) details](https://code.visualstudio.com/updates/v1_93#_github-copilot)