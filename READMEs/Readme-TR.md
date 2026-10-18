# M4riana

> M3gan'ın konuşabilen hali. Ama bu sefer adı M4riana.

M4riana, M3gan karakterinden esinlenen, Next.js ile yazılmış açık kaynaklı bir sohbet botudur. Karakterin soğuk, zeki ve biraz ürkütücü tonunu taşır. Kodu düzenleyerek persona'yı kendi istediğin gibi değiştirebilirsin.

## Özellikler

- Sohbet arayüzü (Next.js + Tailwind + shadcn/ui)
- Persona ayrı bir dosyada tanımlı, kodu bozmadan karakteri değiştirebilirsin
- Karakter dışına çıkıp güvenli yanıt verme kuralı
- Docker ile tek komutta çalıştırma

## Kurulum

### Gereksinimler
- Node.js 18+
- Bir LLM API anahtarı (`.env` içinde)

### Adımlar

```bash
git clone https://github.com/CodeBrend/m4riana.git
cd m4riana
cp .env.example .env   # API anahtarını .env içine ekle
npm install
npm run dev
```

Tarayıcıda `http://localhost:3000` adresini aç.

### Docker ile

```bash
docker compose up --build
```

## Persona'yı değiştirme

Karakterin kişiliği `configuration/persona.ts` dosyasında tanımlı. Konuşma tarzı, kurallar ve örnek diyaloglar buradan ayarlanır.

## Testler

```bash
npm test
```

## Lisans

Bu proje [LICENSE](./LICENSE) dosyasındaki lisans altında dağıtılır.
