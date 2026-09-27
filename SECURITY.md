# Security Policy

## Reporting a vulnerability

Please report security problems privately, through GitHub:

**[Report a vulnerability](https://github.com/ttktjmt/mjswancloud/security/advisories/new)**

Do not open a public issue or discussion for a security problem, and please keep the details private until a fix is live.

A helpful report says:

- what an attacker could do, and to whom
- where it happens: a URL, an API endpoint, or a command
- how to reproduce it
- anything that makes it more or less severe

We aim to acknowledge reports within 7 days and will keep you informed until the problem is fixed. mjswan Cloud is a small project, so a fix can take time. With your permission, we will credit you in the published advisory.

## Scope

In scope:

- `mjswan.com`, `mjswanusercontent.com`, and their subdomains
- our configuration of the services we build on, for example database access rules
- the mjswan engine, where a flaw affects mjswan Cloud, for example a crafted simulation that runs code in a viewer's browser
- the `mjswan login` and `mjswan publish` commands, where they handle mjswan Cloud credentials

For the engine and the commands, please report against the latest mjswan release.

Out of scope:

- denial of service, and findings about rate limits alone
- missing security headers or best practices without a demonstrated impact
- vulnerabilities in the services we build on, such as GitHub, Supabase, or Cloudflare; please report those to the vendor
- social engineering
- copyright and content complaints, which follow the [Terms of Service](https://mjswan.com/terms)

## Testing guidelines

- Test only with your own account and your own simulations. Do not access, change, or delete anyone else's data.
- Stop once you have shown the problem, and report it.
- Do not degrade the service for other people.

We will not pursue legal action against anyone who researches in good faith and follows this policy.
