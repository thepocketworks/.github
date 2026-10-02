<!-- # links ------------------------------------------------------------- # -->

[email]: mailto:baginskioss@proton.me

<!-- # contact ----------------------------------------------------------- # -->

## Security Contact

> [!WARNING]\
> **Please do not open a public GitHub Issue for
> security vulnerabilities**\
> If you believe you have found a **security vulnerability**, a
> security-related bug, or any other issue that could compromise the
> security, privacy, or integrity of a project, please report it
> **directly by email:**
>
> #### [`baginskioss@proton.me`][email]

The security of my projects and the people who use them is
important to me.

Security issues should not be disclosed publicly before they have been
investigaated and, when applicable, fixed. Publicly reporting a
vulnerability may expose users, projects, or other systems to
unnecessary risk.

For security-related reports, please use the email above so that I can
review the report privately and work with you on an appropriate
response.

<!-- # what to report ---------------------------------------------------- # -->

## What to Report

Please contact me if you discover something that could have a security
impact, including but not limited to:

- Authentication or authorization vulnerabilities.
- Unauthorized access to data or functionality.
- Exposure of sensive information.
- Credential, token, API key, or secret leakage.
- Remote code execution.
- Command injection.
- Code injection.
- Cross-site scripting (XSS).
- SQL injection or other injection vulnerabilities.
- Path traversal or arbitrary file access.
- Server-side request forgery (SSRF).
- Insecure deserialization.
- Privilege escalation.
- Security-related dependency vulnerabilities.
- Unsafe default configurations.
- Vulnerabilities in build, release, or distribution processes.
- Supply-chain security issues.
- Denial-of-service vulnerabilities with meaningful security impact.
- Any other issue that could reasonably compromise users, maintainers,
  ifrastructure, or project data.

If you are unsure whether something qualifies as a security
vulnerability, **please report it privately anyway**. I would rather
review a report that turns out not to be a security-related than have
a potentially serious vulnerability disclosed publicly.

<!-- # what not to do ---------------------------------------------------- # -->

## Please Do Not

To help protect users and the projects, please do not:

- Open a public Issue to report a security vulnerability.
- Publicly disclose the vulnerability before it has been investigated.
- Publish proof-of-concept code that enables exploration before a fix
  or mitigation is available.
- Access, modify, delete, or exfiltrate data that does not belong to you.
- Perform actions that could negatively affect other users or systems.
- Conduct denial-of-service atttacks or intentionally degrade
  project availability.
- Use social engineering against project contributors, maintainers,
  or users.
- Test vulnerabilities against infrastructure or services that you do
  not own or have explicit permission to test.

When demonstrating a vulnerability, please use the **minimum amount of
testing necessary** to reproduce and validate the issue.

<!-- # report a vulnerability -------------------------------------------- # -->

## Reporting a Vulnerability

When reporting a vulnerability, please provide as much relevant
information as possible.\
A useful security report should include:

- **Project:** The affectted project or repository.
- **Affected version:** The version, commit, or branch where the
  vulnerability was found.
- **Vulnerability type:** A short description of the security issue.
- **Impact:** What an attacker could potentially do by exploiting
  the vulnerability.
- **Reproduction steps:** Clear steps to reproduce the issue.
- **Proof of concept:** If available, a minimal proof of concept
  demonstrating the vulnerability.
- **Environment:** Relevant operating system, runtime, browser,
  configuration, or deployment information.
- **Suggested mitigation:** If you have an idea for fixing or mitigating
  the issue, please include it.

Please avoid including real credentials, private information, production
secrets, or personal data in your report.\
If sensitive information is required to reproduce the issue, please
describe what is needed rather than sending the sensitive information
itself.

<!-- # response process -------------------------------------------------- # -->

## What Happens After a Report

After receiving a security report, I will review the information and
determine whether the reported issue represents a security vulnerability.

Depending on the situation, the process may include:

1. Acknowledging receipt of the report.
2. Reviewing and reproducing the reported behavior.
3. Assessing the potential impact and severity.
4. Identifying affected versions or components.
5. Developing and testing a fix or mitigation.
6. Releasing the necessary changes.
7. Publishing a security advisory or other appropriate disclosure,
   when necessary.

The exact process and timeline may vary depending on the complexity and
severity of the vulnerability.\
I may contact you by email if additional information is required.

<!-- # disclosure -------------------------------------------------------- # -->

## Coordinated Disclosure

I appreciate responsible and coordinated disclosure of security
vulnerabilities.\
If a vulnerability is confirmed, I will work toward addressing it before
public disclosure whenever reasonably possible.\
Please allow sufficient time for investigation, development, testing and
release of a fix before publicly disclosing the vulnerability.

When appropriate, security fixes may be accompanied by a security
advisory, release notes, changelog entry, or other public communication.\
If you report a vulnerability and would like to be credited for the
discovery, please include the name or handle you would like to use
in the report.

I will respect reasonable requests regarding attribution.

<!-- # severity ---------------------------------------------------------- # -->

## Severity

Security issues may be evaluated according to their potential impact,
exploitability, affected users, and the amount of access an attacker
could obtain.\
As a general guideline, issues may be considered:

- **Critical** - Vulnerabilities that could result in severe compromise
  of systems, sensitive data, or a large number of users.
- **High** - Vulnerabilities that could provide significant unauthorized
  access, execution, or disclosure.
- **Medium** - Vulnerabilities with a meaningful security impact but
  requiring additional conditions or having more limited consequences.
- **Low** - Security issues with limited impact or exploitability.

Severity is evaluated on a case-by-case basis. The final classification
may depend on the specifc project, deployment model, affected component,
and realistic attack scenario.

<!-- # dependencies ------------------------------------------------------ # -->

## Dependency Vulnerabilities

Some projects may depend on third-party libraries, packages, runtimes,
or other external components.\
If you discover that a project uses a vulnerable dependency, please
report it privately when the vulnerability creates a meaningful
security risk to the project or it users.

Where possible, dependency vulnerabilities will be addressed through
dependency updates, configuration changes, patches, or other
appropriate migrations.

<!-- # accidental disclosure --------------------------------------------- # -->

## Accidental Disclosure

If you accidentally discover credentials, API keys, tokens, private
information, or other sensitive data associated with one of my projects,
please **do not use, publish, or redistribute it**.

Report the exposure privately at:
[**`baginskioss@proton.me`**][email].

Please include enough information for me to identify the affected project
and determine what needs to be revoked, removed, or changed.

<!-- # public issues ----------------------------------------------------- # -->

## Public Issues

GitHub Issues are intended for general bugs, feature requests, questions,
an other non-sensitive project discussions.\
**Security vulnerabilities should never be reported through
public issues.**

If an issue contains sensitive security information, please contact me
privately instead.\
If a security vulnerability is accidentally disclosed through a public
Issue, I may remove or restrict the information where possible and move
the discussion to a private channel.

<!-- # scope ------------------------------------------------------------- # -->

## Scope

This security policy applies to security vulnerabilities affecting the
projects covered by this repository and their intended functionality.

Third-party services, dependencies, infrastructure, websites, or
applications that are not maintained by me may have their own security
policies and reporting procedures.

If you believe a vulnerability belongs a third-party component, plase
report it to the appropriate maintainer or security contact as well.

<!-- # reponsible research ----------------------------------------------- # -->

## Reponsible Security Research

I appreciate the work of security researchers and developers who help
identify and responsibly report vulnerabilities.\
Good-faith security research helps make open-source software safe
for everyone.

If you follow this policy, avoid unnecessary harm, respect user privacy,
and report vulnerabilities privately, I will treat your report as a
resposible security disclosure.

Thank you for takign the time to help improve the security of
my projects.

<!-- # contact ----------------------------------------------------------- # -->

## Contact

> [!WARNING]\
> **Do not open a GitHub Issue for security vulnerabilities.\
> Contact me directly by email.**

For all security-related reports and questions, please contact:

#### [`baginskioss@proton.me`][email]
