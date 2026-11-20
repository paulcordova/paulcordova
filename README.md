<img src="banner-EN.png" alt="Legacy .NET · Untangle, don't rewrite" width="100%">

# Paul Córdova

**Maintainer of EntitySpaces.** I modernize legacy .NET systems: business logic out of the forms, data layer on EntitySpaces, interface on Wisej.NET.

[netstep.cl/wisej](https://netstep.cl/wisej) · Viña del Mar, Chile

---

## Why the work looks like this

Two things are true of almost every legacy .NET system I open:

1. **The business logic is in the forms.** Not in classes, not in a service layer — in the event handlers of a screen somebody wrote in 2009 and nobody has dared to touch since. That copy is the only one that exists.
2. **A rewrite throws away decisions nobody wrote down.** Fourteen years of edge cases, exceptions agreed with the client over the phone, and reports that only work because of a `WHERE` clause added in a hurry.

So the work is not to rewrite. It is to move.

## How a migration runs

| Step | What happens |
|---|---|
| **1. Inventory** | What each screen does, which queries it fires, which rules it applies. |
| **2. Relocation** | The logic leaves the forms and moves into an entity layer that can be read and tested. |
| **3. Interface** | The screens move to Wisej.NET and work again in Chrome, Firefox and Edge — no compatibility mode, no front-end rewrite. |
| **4. Repeat** | The same procedure, module by module, with the system running in production. |

## What I maintain

**[EntitySpaces](https://github.com/paulcordova/EntitySpaces)** — an ORM that generates the data layer from the schema, so it survives every change in the database. BSD 3-Clause.

- NuGet: [EntitySpaces.ORM.*](https://www.nuget.org/profiles/paulcordova) for SQL Server, PostgreSQL, MySQL, SQLite and Oracle
- Targets .NET Framework 4.8 through .NET 10
- Studio: schema-to-code, with metadata for length, precision, computed and concurrency columns

**Wisej.NET** — [official partner for Latin America](https://docs.wisej.com/license/services/international-resellers) since 2019. WinForms-shaped applications, running in the browser.

## Proof, not adjectives

- In 2012 I built the system a Chilean winery uses to manage grape purchase and bulk wine export contracts. It is still in production.
- EntitySpaces is not a sample: five database engines on one API surface, each with its own test suite.
- The [benchmark](https://github.com/paulcordova/EntitySpaces-vs-NET-ORMs-Benchmarks) puts it against Dapper, EF Core and EF6 on the same relational workload — performance, memory and cold start, published rather than claimed.

## Where to look

| Repository | What it shows |
|---|---|
| [EntitySpaces](https://github.com/paulcordova/EntitySpaces) | The maintained line: source, Studio, and the .NET Framework 4.8 → .NET 10 targets |
| [EntitySpaces-vs-NET-ORMs-Benchmarks](https://github.com/paulcordova/EntitySpaces-vs-NET-ORMs-Benchmarks) | BenchmarkDotNet against Dapper, EF Core and EF6 |
| [EntitySpaces_Sqlite_Wisej_Sample](https://github.com/paulcordova/EntitySpaces_Sqlite_Wisej_Sample) | EntitySpaces + Wisej, end to end, zero infrastructure |
| [EntitySpaces_PostgreSQL_Wisej_Sample](https://github.com/paulcordova/EntitySpaces_PostgreSQL_Wisej_Sample) | The same application against PostgreSQL |
| [Winforms2WiseJ](https://github.com/paulcordova/Winforms2WiseJ) | WinForms controls next to their Wisej equivalents, to check what actually survives the move |

## Working with me

I work alone, and that is deliberate: the person who designs is the person who builds, and answers the same week. There is no project manager between the problem and the solution.

The first step is always the same: **a two-week diagnostic, fixed price**, with a report you can take to your management. If the numbers do not convince you, you keep the report.

[Modernization service](https://netstep.cl/modernizacion-legacy/) · [EntitySpaces](https://netstep.cl/entityspaces/) · [Book a call](https://calendly.com/paulcordova)

---

*If EntitySpaces saved you a rewrite, [you can support its maintenance](https://netstep.cl/entityspaces/support/).*
