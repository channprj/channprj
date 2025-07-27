## Park Hee Chan (CHANN)

```py
import json
from dataclasses import dataclass, field
from typing import Dict, List


@dataclass
class Profile:
    name: str = "Park Hee Chan"
    description: str = "Software Engineer over 9 years"
    nickname: str = "CHANN"
    job: str = "👨🏻‍💻 Software Engineer"
    nationality: str = "🇰🇷 South Korea"
    resume: Dict[str, str] = field(
        default_factory=lambda: {
            "english": "https://resume.chann.kr/en/",
            "korean": "https://resume.chann.kr/ko/",
        }
    )
    skills: List[str] = field(
        # fmt: off
        default_factory=lambda: [
            "python", "go", "typescript",
            "postgres", "mysql", "redis", "kafka",
            "devops", "docker", "kubernetes", "automation",
            "homelab", "keyboard",
            "finance", "investment",
            "hci", "etc."
        ]
    )
    education: List[Dict[str, str]] = field(
        default_factory=lambda: [
            {"field": "💻 Computer", "type": "B.E."},
            {"field": "🧠 Brain", "type": "B.Sci."},
        ]
    )
    hobbies: List[str] = field(
        # fmt: off
        default_factory=lambda: [ "🥾 Hiking", "🎾 Tennis", "🚴🏻 Cycling", "💪🏻 Fitness"]
    )
    social: Dict[str, str] = field(
        default_factory=lambda: {
            "blog": "https://blog.chann.kr",
            "digital-garden": "https://garden.chann.dev",
            "instagram": "https://instagram.com/channprj",
            "linkedin": "https://linkedin.com/in/channprj",
            "x": "https://x.com/channprj",
            "fediverse": "https://mastodon.social/@chann",
        }
    )

    def json(self):
        return json.dumps(self, default=lambda o: o.__dict__)


# Example usage
profile = Profile()
print(profile.json())
```

- 👨🏻‍💻 Software Engineer
- 🇰🇷 From South Korea
- 🥰 Like Hiking 🥾 and Cycling 🚴🏻‍♂️ and Tennis 🎾
- 🎓 B.E. in 💻 and B.Sci. in 🧠
- 🏷 go, py, ts, devops, docker, k8s, automation, rpi, homelab, keyboard, investment, finance, hci, etc. 
- 🌐 https://blog.chann.kr
- 🗄️ https://garden.chann.dev
- Resume: [English :us:](https://resume.chann.kr/en) or [한국어 :kr:](https://resume.chann.kr/ko)

<br />
<p align="center">
  <a href="https://blog.chann.kr"><img src="https://img.shields.io/badge/blog-blog.chann.kr-202020.svg" alt="Blog" /></a>
  <a href="https://x.com/channprj"><img src="https://img.shields.io/badge/X-channprj-000000.svg?style=flat&logo=x" alt="X" /></a>
  <a href="https://instagram.com/channprj"><img src="https://img.shields.io/badge/Instagram-channprj-e1306c.svg?style=flat&logo=instagram" alt="Instagram" /></a>
  <a href="https://kr.linkedin.com/in/channprj"><img src="https://img.shields.io/badge/LinkedIn-channprj-0077b5.svg?style=flat&logo=linkedin" alt="LinkedIn" /></a>
  <a href="https://mastodon.social/@chann"><img src="https://img.shields.io/mastodon/follow/000219287" alt="Fediverse" /></a>
</p>
<!--

<p align="center">
  <a href="https://github.com/anuraghazra/github-readme-stats">
    <img align="left" src="https://github-readme-stats.vercel.app/api?username=channprj&count_private=true&show_icons=true" />
  </a>
  <a href="https://github.com/anuraghazra/github-readme-stats">
    <img align="left" src="https://github-readme-stats.vercel.app/api/top-langs/?username=channprj&layout=compact&count_private=true&hide=css,html,vim script" />
  </a>
</p>
-->
