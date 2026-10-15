# Geoportal de Zoneamento — Jaguariúna (Lei Complementar nº 409/2024)

Geoportal oficial da **Prefeitura Municipal de Jaguariúna** com o zoneamento de uso e ocupação do solo da **Lei Complementar nº 409/2024 (Anexo III)**, a expansão urbana e a área rural do município.

**Acesse:** https://mirianniz-debug.github.io/LeiComplementar409/

## O que o geoportal mostra

- **Zonas de uso** (ZR, ZPR, ZC, ZPPH, ZI e ZEIS), com as cores do mapa oficial e a área de cada uma.
- **Demais áreas do município:** área urbana sem zona definida no Anexo III, expansão urbana, área rural e áreas sem classificação.
- **AIA** (Área de Interesse Ambiental): **prevalece sobre qualquer zona ou classificação**. A consulta destaca que se trata de AIA e cita a classe que existiria por baixo.
- **Base territorial:** limite municipal (IBGE), corredores de comércio e serviços (CCS), ferrovia e hidrografia.
- **Consulta de um local:** clique no mapa, digite um endereço ou latitude e longitude para saber a zona, o perímetro, se está em AIA e o nível de confiança da resposta.

## Como ler a confiança

| Nível | Significado |
|---|---|
| **Alta** | Zona ou AIA do Anexo III (LC 409/2024), ou classificação rural / expansão urbana da LC 373/2022 (Plano Diretor). |
| **Média** | Ponto a até 30 m de uma divisa entre polígonos (zonas, AIA ou outras classificações). |
| **Baixa** | Área urbana sem zona definida no Anexo III, ou fora das camadas disponíveis. |

## Aviso

Em Área de Interesse Ambiental (AIA) prevalece a AIA sobre qualquer zona ou classificação. Onde o Anexo III e a LC 373/2022 (Plano Diretor) divergem, o geoportal mostra a classificação da **LC 373/2022**, que prevalece em caso de conflito (art. 217, parágrafo único, da LC 409/2024).

Consulta **informativa**. O desenho do Anexo III não é georreferenciado pela Prefeitura; o mapa foi ajustado a uma base real (OpenStreetMap, limite do IBGE e hidrografia) com erro estimado de até 30 m. Perto de divisas, confirme com a Secretaria de Planejamento Urbano. Esta consulta **não substitui** a certidão de uso e ocupação do solo.

## Fontes

- Lei Complementar nº 409/2024, Anexo III — Zoneamento de Uso e Ocupação do Solo (Prefeitura de Jaguariúna).
- IBGE — limite municipal.
- Lei Complementar nº 373/2022 (Plano Diretor de Jaguariúna) — classificação das áreas urbana, de expansão urbana e rural.
- Mapa base: © colaboradores do OpenStreetMap; Esri; OpenTopoMap.

## Estrutura

```
index.html        página do geoportal (HTML, CSS e JavaScript, sem etapa de build)
data/             camadas em GeoJSON (WGS84)
images/           brasão do município
preview.png       prévia
```

Tecnologias: [Leaflet](https://leafletjs.com/) e HTML/CSS/JavaScript puro.

Elaboração cartográfica: Engª Mirian Niz.

