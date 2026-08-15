<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:0d1117&height=10&section=header" width="100%" />

</div>

```rust
#![allow(dead_code)]
//! src/ababil.rs — zsh @ arch — 100% local-first
//! `cargo run --bin ababil` — Full-Stack Robotics Engineer (in progress)

#[derive(Debug)]
struct Ababil {
    name: &'static str,
    role: &'static str,
    location: &'static str,
    focus: &'static [&'static str],
    philosophy: &'static str,
}

#[derive(Debug)]
struct Stack {
    lang: &'static [&'static str],
    frontend: &'static [&'static str],
    backend: &'static [&'static str],
    infra: &'static [&'static str],
    db: &'static [&'static str],
}

struct Links {
    portfolio: &'static str,
    email: &'static str,
    github: &'static str,
}

const ABABIL: Ababil = Ababil {
    name: "Ababil Mustaqim",
    role: "Full-Stack Robotics Engineer (in progress)",
    location: "Batam, ID",
    focus: &["Robotics Software", "Embedded", "AI/ML", "System Design"],
    philosophy: "local-first · self-hosted · build from source",
};

const STACK: Stack = Stack {
    lang: &["Python", "TypeScript", "JavaScript", "Rust", "Java", "Kotlin"],
    frontend: &["Vue", "Nuxt", "Svelte", "Astro", "Tailwind"],
    backend: &["Flask", "Express", "Node.js"],
    infra: &["Docker", "Nix", "Traefik", "Linux", "systemd"],
    db: &["PostgreSQL", "MySQL", "Redis"],
};

impl Ababil {
    const fn currently(&self) -> &'static str {
        "System Design · Rust & Embedded · AI/ML pipelines"
    }

    const fn links(&self) -> Links {
        Links {
            portfolio: "https://ababil-is-no.fun",
            email: "ababilmustaqim@proton.me",
            github: "https://github.com/zuckdorsey",
        }
    }
}

fn main() {
    let me = &ABABIL;
    println!("{} — {} @ {}", me.name, me.role, me.location);
    println!("currently: {}", me.currently());
    println!("philosophy: {}", me.philosophy);
}
```

```sh
# ~/ababil $ cargo run --quiet
Ababil Mustaqim — Full-Stack Robotics Engineer (in progress) @ Batam, ID
currently: System Design · Rust & Embedded · AI/ML pipelines
philosophy: local-first · self-hosted · build from source — ship to prod.

# quick links
→ portfolio  https://ababil-is-no.fun
→ email      ababilmustaqim@proton.me
→ github     github.com/zuckdorsey
→ location   Batam City, Indonesia

# stack
→ lang     Python · TypeScript · Rust · Java/Kotlin
→ fe       Vue/Nuxt · Svelte · Astro · Tailwind
→ infra    Docker · Nix · Traefik · Linux · systemd
```

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/zuckdorsey/zuckdorsey/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/zuckdorsey/zuckdorsey/output/github-contribution-grid-snake-light.svg">
  <img alt="snake" src="https://raw.githubusercontent.com/zuckdorsey/zuckdorsey/output/github-contribution-grid-snake.svg">
</picture>

<!-- snake: 4 variants on /output branch — github · github-dark · github-light · purple -->
<!-- purple alt: https://raw.githubusercontent.com/zuckdorsey/zuckdorsey/output/github-contribution-grid-snake-purple.svg -->
