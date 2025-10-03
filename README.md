COMPANY: CODTECH IT SOLUTIONS

NAME: OMIKA JENA

INTERN ID: CT04DY2062

DOMAIN: AUTOMATION TESTING

DURATION: 4 WEEKS

MENTOR: NEELA SANTHOSH

# 📌 Project Description: CI/CD Pipeline with Automated Testing

## 🔹 Overview

This project demonstrates how to **integrate automated tests into a CI/CD pipeline** using **GitHub Actions** and **Jenkins**. Automated testing ensures that every change in the codebase is validated quickly, reducing bugs and improving reliability.

The setup uses a simple Python project (`src/calculator.py`) with unit tests (`tests/`) written in **pytest** to illustrate how pipelines can be configured to automatically run tests, generate reports, and publish results.


## 🔹 Objectives of the Task

* Configure a CI/CD pipeline that runs **automated tests** on every commit and pull request.
* Generate **JUnit XML** and **HTML test reports** for better visibility.
* Provide support for **GitHub Actions** (cloud-based CI/CD) and **Jenkins** (self-hosted CI/CD).
* Deliver a **ready-to-use project skeleton** that can be extended for real-world applications.

## 🔹 Tools Used

1. **GitHub Actions**

   * Cloud-based CI/CD solution built into GitHub.
   * Executes workflows defined in `.github/workflows/ci.yml`.
   * Suitable for projects already hosted on GitHub.

2. **Jenkins**

   * Open-source automation server widely used in enterprises.
   * Uses a `Jenkinsfile` to define declarative pipelines.
   * Provides flexibility with plugins like **JUnit** and **HTML Publisher** for test reporting.

3. **pytest**

   * Python testing framework used to write and run unit tests.
   * Extended with `pytest-html` for HTML reports and `pytest-cov` for coverage reports.

4. **Reporting Tools**

   * **JUnit XML**: Allows CI tools to parse and display test results.
   * **HTML Report**: Developer-friendly, detailed test execution report.


## 🔹 Where It Is Used

* **Agile Teams**: Quick validation of frequent commits.
* **Enterprises**: Ensures quality and stability in mission-critical applications.
* **Open-Source Projects**: Guarantees consistency in contributions from different developers.
* **DevOps Workflows**: Core part of continuous delivery pipelines.

## 🔹 How to Use It

1. **Clone & Push**

   * Copy this project structure into a new GitHub repository.
   * Push changes to trigger the **GitHub Actions** workflow automatically.

2. **GitHub Actions**

   * Open the **Actions** tab in GitHub.
   * Download test reports from workflow **artifacts**.

3. **Jenkins**

   * Create a new **Pipeline job** pointing to this repo.
   * Jenkins will run tests, publish **JUnit results**, and display the **HTML report**.

4. **Extend the Project**

   * Add your application code under `src/`.
   * Write tests in the `tests/` folder.
   * The pipeline will automatically validate your new code.

## 🔹 Benefits

✅ Automated and repeatable testing

✅ Early detection of bugs

✅ Reports for better debugging & tracking

✅ Works with both GitHub Actions & Jenkins

✅ Scalable for real-world projects

## 🔹 Conclusion

This project provides a **practical demonstration of CI/CD pipelines with automated testing**. By integrating GitHub Actions or Jenkins with pytest, developers can ensure high-quality code, speed up release cycles, and build reliable applications. The setup can be extended to include linting, Docker builds, deployment steps, or advanced monitoring — making it a strong foundation for modern DevOps workflows.


