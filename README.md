# Awesome GPU Cloud Russia [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

<img src=".github/banner.jpg" alt="Awesome GPU Cloud Russia — где арендовать облачную GPU для нейросетей из России" width="100%">

> Где арендовать облачную видеокарту (GPU) для нейросетей из России: Stable Diffusion, ComfyUI, инференс LLM, обучение. Честный, проверяемый список с источниками.
>
> *English: a curated list of cloud GPU rental options available from Russia for AI/ML. English summary at the [bottom](#english-summary).*

**Последнее обновление: 2026-11-11.**

**Раскрытие интересов:** автор списка делает сервис [gpu.nz](https://gpu.nz). Он включён в список и помечен как «сервис автора списка». Остальные сервисы описаны по их собственным страницам; ссылки на источники приведены. Если вы нашли ошибку, откройте PR (см. [CONTRIBUTING.md](CONTRIBUTING.md)).

## Принципы

- Цена указывается только если она найдена на странице самого провайдера; тогда рядом стоит пометка «по данным сайта на октябрь 2026» и ссылка. Иначе дана ссылка на страницу тарифов.
- То, что нельзя проверить без аккаунта (например, оплата из РФ у зарубежных сервисов), помечено «не проверено».
- Цены в рублях у российских облаков часто указаны «от»: итог зависит от конфигурации (CPU, RAM, диск, трафик) и НДС.

## Содержание

- [Российские облака и хостинги](#российские-облака-и-хостинги)
- [gpu.nz (сервис автора списка)](#gpunz-сервис-автора-списка)
- [Международные сервисы](#международные-сервисы)
- [Бесплатные варианты](#бесплатные-варианты)
- [Как выбрать видеокарту: сколько VRAM нужно](#как-выбрать-видеокарту-сколько-vram-нужно)
- [Тарификация: посекундная, поминутная, почасовая, помесячная](#тарификация)
- [Способы оплаты](#способы-оплаты)
- [Полезные инструменты](#полезные-инструменты)
- [FAQ](#faq)
- [English summary](#english-summary)
- [Участие](#участие) · [Лицензия](#лицензия)

## Российские облака и хостинги

Колонка «Оплата из РФ» отражает то, что указано на сайте провайдера; «не проверено» значит, что на проверенных страницах способы оплаты не перечислены.

| Сервис | Что есть | Тарификация | Оплата из РФ | Ссылка |
|---|---|---|---|---|
| Selectel | Облачные и выделенные GPU-серверы: Tesla T4, A2, A30, A100, A2000, A5000, RTX 4090 и др. (список на странице). Цены GPU на странице не загружаются, смотрите калькулятор | Час, сутки, месяц (по данным сайта) | Банковская карта, ЮMoney, счёт для юрлиц (по данным сайта) | [GPU-серверы](https://selectel.ru/services/cloud/servers/gpu/) · [тарифы](https://selectel.ru/prices/) |
| Yandex Cloud | Виртуальные машины с GPU NVIDIA V100 и A100 (по данным сайта) | Не проверено; см. страницу цен | Не проверено | [Compute Cloud](https://yandex.cloud/ru/docs/compute/concepts/gpus) · [цены](https://yandex.cloud/ru/docs/compute/pricing) |
| VK Cloud | GPU для ВМ, Kubernetes и bare metal; по обзорам прессы до H200 и дробные vGPU. Прямая страница GPU недоступна для автоматической проверки | Не проверено | Не проверено | [Документация GPU](https://cloud.vk.com/docs/computing/gpu) · [VK Cloud](https://cloud.vk.com/) |
| Cloud.ru (Evolution) | Виртуальные машины с GPU; страница продукта «Вычислительные мощности с GPU» | Час/сутки/месяц в калькуляторе общих ВМ; для GPU не проверено | Не проверено | [Cloud.ru GPU](https://cloud.ru/products/vychislitelnyye-moschnosti-s-gpu) |
| immers.cloud | Каталог GPU от RTX 2080 Ti до H100/H200; шаблоны ВМ | Посекундная, бесплатная «пауза» (по данным сайта) | Предоплата от 100 ₽; способы оплаты на странице не перечислены, не проверено | [immers.cloud](https://immers.cloud/) · [GPU](https://immers.cloud/gpu/) |
| Timeweb Cloud | GPU-серверы: GTX 1080 / 2080 Ti, RTX 3080/3090/4090, A2/A30/A4000/A5000/A6000, T4; H100/H200/A100 по предзаказу (по данным сайта) | Списание раз в час; тарифы месячные (по данным сайта) | Мин. пополнение от 5 000 ₽; приём карт МИР/Visa/Mastercard/UnionPay указан в разделе о безопасности платежей | [Timeweb GPU](https://timeweb.cloud/services/gpu) |
| REG.RU (Облако) | Раздел GPU в облаке REG.RU; содержимое страницы не удалось прочитать автоматически | Не проверено | Не проверено | [REG.RU Cloud](https://www.reg.ru/cloud/gpu) |
| HOSTKEY | Выделенные GPU-серверы и GPU VPS: RTX 3080/3090/4090/5090, A5000/A6000, A100, H100 (часть по предзаказу) | Почасовая и помесячная оплата (по данным сайта) | В подвале сайта указаны Visa/Mastercard/МИР, ЮMoney, СБП и банки; полный список на странице «Оплата» не проверен | [HOSTKEY GPU](https://hostkey.ru/gpu-dedicated-servers/) |
| ITGLOBAL | AI Cloud на vGPU (по сообщениям прессы 2023 г., карты A800 в VMware) | Pay as you go (по сообщениям прессы) | Не проверено | [ITGLOBAL](https://itglobal.com/ru-ru/) |
| MWS (облако МТС) | Облачные сервисы МТС Web Services; GPU-предложение не проверено | Не проверено | Не проверено | [MWS](https://mws.ru/) |

### Цены, найденные на страницах провайдеров

По данным сайта на октябрь 2026. Это стартовые цены («от»), конкретная конфигурация может стоить иначе.

| Сервис | Конфигурация | Цена | Источник |
|---|---|---|---|
| immers.cloud | 1× RTX 3090 / 1× RTX 4090 / 1× A100 / 1× H100 | от 70,7 / 86,7 / 223,0 / 353,0 ₽ в час | [immers.cloud](https://immers.cloud/) |
| HOSTKEY | 1× RTX 4090 24 ГБ, выделенный сервер | от 37 000 ₽ в месяц | [hostkey.ru](https://hostkey.ru/gpu-dedicated-servers/) |
| HOSTKEY | 1× RTX 3080 10 ГБ / 1× RTX 5090 32 ГБ | 19 000 / 61 900 ₽ в месяц | [hostkey.ru](https://hostkey.ru/gpu-dedicated-servers/) |

У Selectel, Timeweb Cloud, Yandex Cloud и Cloud.ru цены на GPU нужно смотреть в калькуляторе на их сайтах (ссылки в таблице выше).

## gpu.nz (сервис автора списка)

> Раскрытие: gpu.nz делает автор этого списка.

| Сервис | Что есть | Тарификация | Оплата из РФ | Ссылка |
|---|---|---|---|---|
| **gpu.nz** (сервис автора списка) | Каталог около 90 конфигураций, от RTX 3060 до H100; шаблоны ComfyUI, Stable Diffusion Forge, Open WebUI + Ollama, vLLM, Whisper, Jupyter | Поминутная: цена часа делится на 60; цена фиксируется при запуске; GPU не тарифицируется на остановленном сервере, диск тарифицируется пока существует | СБП из банков РФ; криптовалюта через CryptoBot (USDT, TON, BTC и др.). Счета для юрлиц: «скоро» | [gpu.nz](https://gpu.nz) · [цены](https://gpu.nz/pricing) · [шаблоны](https://gpu.nz/templates) |

Цены на gpu.nz зависят от конкретного сервера и обновляются каждую минуту; актуальные значения смотрите на [странице цен](https://gpu.nz/pricing). По данным сайта на октябрь 2026, стартовые цены в каталоге: RTX 3060 12 ГБ от 7,20 ₽/ч, RTX 4090 от 33 ₽/ч, A100 SXM4 80 ГБ от 126 ₽/ч, H100 SXM 80 ГБ от 300 ₽/ч. Сайт сообщает: при нехватке баланса на минуту сервер и диски удаляются; возвраты только в случаях, предусмотренных законом.

## Международные сервисы

Мы не проверяли, принимают ли эти сервисы платежи из РФ: это зависит от банка, карты и политики сервиса на текущий момент. Везде «не проверено».

| Сервис | Что есть | Тарификация | Оплата из РФ | Ссылка |
|---|---|---|---|---|
| RunPod | Pods, Serverless, кластеры; GPU от RTX 4090 до H100/H200/B300 (по данным сайта) | Почасовая или посекундная (переключатель на странице цен) | Не проверено | [цены](https://www.runpod.io/pricing) |
| Lambda | GPU-облако для ИИ | См. страницу цен | Не проверено | [цены](https://lambda.ai/pricing) |
| Modal | Serverless-запуск Python-кода на GPU | См. страницу цен | Не проверено | [цены](https://modal.com/pricing) |
| Paperspace | GPU-машины и ноутбуки | См. сайт | Не проверено | [сайт](https://www.paperspace.com) |
| Together AI | Инференс и дообучение моделей по API | См. страницу цен | Не проверено | [цены](https://www.together.ai/pricing) |
| Lightning AI | Облачные студии с GPU, есть бесплатный уровень | См. сайт | Не проверено | [сайт](https://lightning.ai/) |
| CloudGPU (сервис автора PR) | Аренда RTX 4090/5090 для обучения, инференса и ComfyUI | См. каталог | Не проверено | [сайт и каталог](https://cloudgpu.app/) · [документация](https://cloudgpu.app/docs) |

## Бесплатные варианты

Бесплатные лимиты часто меняются, и ни один из сервисов не гарантирует доступность GPU.

| Сервис | Что есть | Лимиты | Оплата из РФ | Ссылка |
|---|---|---|---|---|
| Google Colab | Ноутбуки Jupyter с GPU | Лимиты не публикуются; ресурсы «не гарантированы и не безграничны», блокнот работает до 12 часов, типы GPU меняются (по FAQ Colab) | Платные планы: не проверено | [Colab](https://colab.google/) · [FAQ](https://research.google.com/colaboratory/faq.html) |
| Kaggle Notebooks | Ноутбуки с GPU (по обзорам: P100 или 2×T4) | По сторонним обзорам, около 30 ч GPU в неделю; сведения о квотах и длине сессии противоречивы, не проверено по официальной документации | Бесплатно | [Kaggle](https://www.kaggle.com/) · [Docs](https://www.kaggle.com/docs/notebooks) |
| Hugging Face Spaces | Демо-приложения; GPU-железо (в т.ч. ZeroGPU) в платных и специальных планах | См. документацию | Не проверено | [Spaces GPU](https://huggingface.co/docs/hub/spaces-gpus) |
| Lightning AI | Бесплатный уровень с кредитами | См. сайт | Не проверено | [Lightning](https://lightning.ai/) |

## Как выбрать видеокарту: сколько VRAM нужно

Оценки приблизительные: веса модели плюс запас 10-30% на KV-кэш, активации и контекст. Реальная потребность зависит от разрешения, длины контекста, batch и движка. Для обучения нужно в разы больше, чем для инференса.

**LLM (инференс), память на веса:**

| Модель | 4-бит | 8-бит | 16-бит (fp16/bf16) | С запасом подойдёт (4-бит / 16-бит) |
|---|---|---|---|---|
| 7B | ~4 ГБ | ~7 ГБ | ~14 ГБ | 8 ГБ / 24 ГБ |
| 13B | ~7 ГБ | ~13 ГБ | ~26 ГБ | 12 ГБ / 40-48 ГБ |
| 34B | ~17 ГБ | ~34 ГБ | ~68 ГБ | 24 ГБ / 80 ГБ |
| 70B | ~35 ГБ | ~70 ГБ | ~140 ГБ | 48 ГБ / 2×80 ГБ |

**Генерация изображений:**

| Модель | 4-бит | 8-бит | 16-бит |
|---|---|---|---|
| SD 1.5 | не применяется | не применяется | 4-6 ГБ |
| SDXL | не применяется | ~8 ГБ (с оптимизациями) | 10-12 ГБ комфортно |
| FLUX.1 (12B) | ~8-10 ГБ (GGUF Q4) | ~14-16 ГБ (fp8) | ~24 ГБ и больше |

Правила: LoRA/QLoRA-дообучение 7B реально на 16-24 ГБ; полное обучение требует многократно больше; для vLLM закладывайте VRAM под KV-кэш.

## Тарификация

- **Посекундная:** платите ровно за время работы. Среди проверенных: immers.cloud, RunPod (переключатель).
- **Поминутная:** gpu.nz (сервис автора списка).
- **Почасовая:** любая начатая единица может округляться вверх; у Timeweb Cloud списание раз в час, у Selectel возможна аренда на час, сутки, месяц.
- **Помесячная:** выгоднее при постоянной нагрузке, у выделенных серверов (HOSTKEY).
- Смотрите отдельно: тарифицируется ли остановленный сервер, диск, трафик.

## Способы оплаты

- СБП, карты РФ, ЮMoney, счёт для юрлиц: у разных провайдеров по-разному (см. таблицы).
- Криптовалюта: у gpu.nz через CryptoBot.
- Зарубежные сервисы: оплата из РФ не проверена, может меняться.

## Полезные инструменты

| Инструмент | Для чего | Ссылка |
|---|---|---|
| Ollama | Простой запуск LLM локально или на сервере | [ollama.com](https://ollama.com) |
| vLLM | Быстрый сервер инференса LLM, OpenAI-совместимый API | [github.com/vllm-project/vllm](https://github.com/vllm-project/vllm) |
| ComfyUI | Узловой интерфейс для Stable Diffusion, SDXL, FLUX | [github.com/comfyanonymous/ComfyUI](https://github.com/comfyanonymous/ComfyUI) |
| Stable Diffusion WebUI Forge | Веб-интерфейс для SD | [github.com/lllyasviel/stable-diffusion-webui-forge](https://github.com/lllyasviel/stable-diffusion-webui-forge) |
| AUTOMATIC1111 WebUI | Классический веб-интерфейс SD | [github.com/AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) |
| text-generation-webui | Веб-интерфейс для запуска LLM | [github.com/oobabooga/text-generation-webui](https://github.com/oobabooga/text-generation-webui) |

## FAQ

**Где арендовать видеокарту для нейросети в России?**
Варианты: российские облака (Selectel, Yandex Cloud, VK Cloud, Cloud.ru, Timeweb Cloud, immers.cloud, HOSTKEY и др.), а также сервис автора списка gpu.nz с поминутной оплатой через СБП или криптовалюту. Сравните таблицы выше: важны модель GPU, тарификация и способ оплаты.

**Сколько стоит аренда RTX 4090?**
Зависит от провайдера и конфигурации. По данным сайтов на октябрь 2026: immers.cloud от 86,7 ₽/ч ([источник](https://immers.cloud/)); HOSTKEY от 37 000 ₽/мес за выделенный сервер ([источник](https://hostkey.ru/gpu-dedicated-servers/)); gpu.nz (сервис автора списка) от 33 ₽/ч ([источник](https://gpu.nz/pricing)). Цены включают разные конфигурации и могут измениться; сверяйтесь с сайтами.

**Чем заменить Google Colab?**
Kaggle Notebooks (бесплатно, с лимитами), Lightning AI, либо платная аренда GPU по минутам или секундам: gpu.nz (шаблон Jupyter), immers.cloud, RunPod (оплата из РФ не проверена).

**Какая видеокарта нужна для Stable Diffusion и SDXL?**
Для SDXL комфортно 12 ГБ VRAM, для FLUX.1 в fp8 нужно примерно 16 ГБ и больше, на 24 ГБ (RTX 3090/4090) удобно. См. таблицу выше.

**Сколько VRAM нужно для LLM 70B?**
Около 35 ГБ на веса в 4-бит и 140 ГБ в fp16, плюс запас на контекст. На практике: 48 ГБ для 4-бит или несколько карт по 80 ГБ.

**Можно ли платить за GPU из России через СБП?**
Да, у части сервисов: например, gpu.nz (сервис автора списка) принимает СБП; HOSTKEY показывает СБП среди способов оплаты. Для остальных проверяйте страницу оплаты.

**Что выгоднее: почасовая аренда или выделенный сервер?**
Для экспериментов и нерегулярной работы почасовая или поминутная; для круглосуточной нагрузки месячная аренда выделенного сервера часто дешевле. Считайте по своей загрузке.

## English summary

A curated, source-linked list of where to rent cloud GPUs from Russia for AI/ML (Stable Diffusion, ComfyUI, LLM inference, training). Russian providers covered: Selectel, Yandex Cloud, VK Cloud, Cloud.ru, immers.cloud, Timeweb Cloud, REG.RU, HOSTKEY, ITGLOBAL, MWS. gpu.nz is the list maintainer's own service and is disclosed as such: per-minute billing, RTX 3060 to H100, top-ups via the Russian SBP instant-payment system or crypto (CryptoBot), with ComfyUI, Forge, Jupyter, Ollama and vLLM templates. International services (RunPod, Lambda, Modal, Paperspace, Together AI, Lightning AI) are linked, but we did not verify whether payments from Russia work ("не проверено"). Free options (Google Colab, Kaggle, Hugging Face Spaces) have changing, non-guaranteed limits. Prices are listed only when found on the provider's own page (October 2026) and always link to the source. The VRAM table gives rough weight sizes (for example, a 70B LLM needs about 35 GB at 4-bit and 140 GB at 16-bit).

## Участие

Предлагайте новые сервисы и исправления через PR: см. [CONTRIBUTING.md](CONTRIBUTING.md).

## Лицензия

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/) Список передан в общественное достояние (CC0 1.0), см. [LICENSE](LICENSE).
