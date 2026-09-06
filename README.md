# my_work_manim

Year-based work archive + exam hall for [Manim](https://www.manim.community/) code.

```
write → test here → passes → main repo
```

## Structure

```
year2026/
├── buffon_needles/    🚧  paper_lib (Paper toolkit) + needle scene
├── line_intersection  ✅  graduated to manim-extras
└── bbox_shift/        ✅  MobjectHelper (get_bbox mixin)
```

## Install & use (Colab)

```python
!apt-get install -y -qq ffmpeg libcairo2-dev libpango1.0-dev texlive-latex-extra \
    fonts-noto-core fonts-noto-extra fonts-beng-extra      # system libs + বাংলা fonts
!pip install -q git+https://github.com/myabdur2121-cpu/my_work_manim-.git
from year2026.buffon_needles.paper_lib import *
import year2026.buffon_needles.scene_construct as sc
!manim -ql {sc.__file__} BuffonNeedlesScene
```

## Rules

- প্রতি folder-এ `__init__.py` থাকবে (package)
- নতুন বছর = নতুন folder + pyproject `include`-এ এক লাইন
- পুরনো বছর read-only history
- Status: 🚧 exam / ✅ passed / ❌ abandoned
