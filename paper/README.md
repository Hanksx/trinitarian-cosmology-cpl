# Teoria Trinitária - Artigo Final
**Organização dos arquivos para publicação**

---

## 📁 Estrutura de Diretórios

```
artigo_final/
├── README.md                          ← Este arquivo
├── codigo/                            ← Scripts Python utilizados
├── dados/                             ← Datasets observacionais
├── figuras/                           ← Todas as figuras e gráficos
│   ├── *.png                          ← 12 figuras cosmológicas
│   └── curvas_ajustadas/              ← 125 curvas de rotação galácticas
└── resultados/                        ← Outputs dos testes
    ├── resultados_lcdm_final.txt
    ├── resultados_trinitario_final.txt
    └── TABELA_COMPARATIVA.md
```

---

## 📊 Figuras Disponíveis

### Cosmologia (12 figuras)

#### Comparação de Modelos
1. **comparacao_Hz.png** - Função de expansão H(z) vs redshift
   - ΛCDM vs Trinitário CPL
   - Dados observacionais: 12 pontos de "cosmic chronometers"
   
2. **comparacao_Hz_relativo.png** - Diferença relativa ΔH/H_ΛCDM
   - Mostra desvios do Trinitário em relação ao ΛCDM
   
3. **comparacao_DL.png** - Distância de luminosidade D_L(z)
   - Usado para ajustar Supernovas Tipo Ia
   
4. **comparacao_DL_relativo.png** - Diferença relativa ΔD_L/D_L,ΛCDM

#### Espaço de Parâmetros (w₀, wₐ)
5. **chi2_heatmap_pantheon.png** - Mapa de calor χ²(w₀, wₐ) apenas com SN
   - Mostra como χ² varia no plano de parâmetros CPL
   
6. **chi2_heatmap_pantheon_bao.png** - Mesmo mapa incluindo BAO
   - BAO restringe significativamente o espaço de parâmetros
   
7. **chi2_contours_pantheon.png** - Contornos de confiança (apenas SN)
   - Níveis: 68%, 95%, 99.7%
   
8. **chi2_contours_pantheon_bao.png** - Contornos (SN + BAO)

#### Contornos de Parâmetros Individuais
9. **contornos_trinitario_Om_w0.png** - Contornos no plano (Ωₘ₀, w₀)
   - Mostra correlação negativa entre densidade de matéria e equação de estado

#### Comparação de Métricas
10. **NLQ_chi2_chi2red.png** - Comparação χ² e χ²_reduzido
    - ΛCDM vs Trinitário por sonda
    
11. **NLQ_AIC_BIC.png** - Critérios de informação
    - AIC (Akaike) e BIC (Bayesian)
    - Ambos favorecem Trinitário
    
12. **NLQ_t0_q0.png** - Quantidades derivadas
    - Idade do universo (t₀) e parâmetro de desaceleração (q₀)

### Galáxias (125 curvas)

**curvas_ajustadas/** contém ajustes individuais para 125 galáxias SPARC:
- Exemplos: NGC3198, NGC2903, DDO064, etc.
- Cada figura mostra:
  * Dados observacionais (pontos com barras de erro)
  * Contribuição bariônica (gás + disco + bojo)
  * Modelo Trinitário completo
  * Resíduos (obs - modelo)

---

## 📈 Resultados Principais

### Cosmologia

**Comparação ΛCDM vs Trinitário CPL:**

| Métrica | ΛCDM | Trinitário | Melhora |
|---------|------|------------|---------|
| χ²_total | 887.55 | **866.53** | -21.0 (2.4%) |
| AIC | 893.55 | **876.53** | -17.0 ✅ |
| BIC | 909.90 | **903.78** | -6.1 ✅ |

**Ganhos por sonda:**
- H(z): -52% (melhora dramática!)
- SN: -1.5%
- BAO: -12%
- CMB: -100% (ajuste perfeito)
- fσ8: +17% (pequena piora - trade-off)

### Galáxias

**Dataset:** 125 galáxias SPARC  
**Performance:**
- RMS teste: 59.7 km/s (dados não vistos)
- Gap: +2.4% (excelente <5%)
- Parâmetros globais: apenas 5
- Parâmetros estruturais fixos: N=4, L=5, Q=4.0

---

## 🔬 Datasets Utilizados

### Cosmologia
- **Supernovas:** Pantheon+SH0ES (1701 SNe Ia) - [pantheon_simplificado.txt]
- **H(z):** Cosmic chronometers (12 medidas) - [dados_hz.txt]
- **BAO:** Oscilações acústicas de bárions (4 medidas) - [bao_dados.txt]
- **fσ8:** Taxa de crescimento de estrutura (9 medidas) - [fs8_dados.txt]
- **CMB:** Prior comprimido em R (parâmetro de deslocamento)

### Galáxias
- **SPARC:** Spitzer Photometry and Accurate Rotation Curves
- **Fonte:** Lelli et al. (2016), AJ, 152, 157
- **URL:** http://astroweb.cwru.edu/SPARC/
- **Galáxias utilizadas:** 125 de alta qualidade (Q≤2)

---

## 🖥️ Código

Os scripts principais estão na pasta `codigo/`:

### Cosmologia
- `fit_lcdm_multisonda_bao_cmb.py` - Ajuste ΛCDM com todas as sondas
- `fit_trinitario_multisonda_bao_cmb.py` - Ajuste Trinitário CPL
- `cosmologia_dados_fallback.py` - Sistema de carregamento de dados
- `modelo_trinitario_cosmologia.py` - Implementação do modelo CPL

### Galáxias
- `ajuste_sparc_otimizado.py` - Ajuste das curvas de rotação
- `comparacao_sparc_modelos.py` - Comparação de modelos
- `analise_estatistica.py` - Estatísticas descritivas

### Visualização
- Scripts para gerar todas as figuras (chi2_maps, contornos, comparações)

---

## 📝 Como Usar

### Reproduzir Resultados Cosmológicos

```bash
cd codigo/
python fit_lcdm_multisonda_bao_cmb.py       # Roda ΛCDM
python fit_trinitario_multisonda_bao_cmb.py # Roda Trinitário
```

### Analisar Galáxias SPARC

```bash
python ajuste_sparc_otimizado.py  # Ajusta 125 galáxias
python analise_estatistica.py     # Estatísticas descritivas
```

### Gerar Figuras

```bash
python cosmo_trinitario_chi2_map.py  # Mapas de χ²
python cosmo_trinitario_chi2_pantheon_bao.py  # Contornos
```

---

## 📄 Citação

Se você usar este código ou resultados, por favor cite:

```bibtex
@article{Silva2025Trinitarian,
  title={Trinitarian Theory: A Phenomenological Framework for Galactic Dynamics and Dark Energy Evolution},
  author={Silva, Nil},
  journal={Em preparação},
  year={2025}
}
```

---

## 📚 Referências Principais

### Dados
- **SPARC:** Lelli et al. (2016), AJ, 152, 157
- **Pantheon+:** Brout et al. (2022), ApJ, 938, 110
- **BAO:** SDSS/BOSS compilações
- **H(z):** Cosmic chronometers (vários autores)

### Modelos
- **CPL parametrization:** Chevallier & Polarski (2001), Linder (2003)
- **ΛCDM:** Perlmutter et al. (1999), Riess et al. (1998)
- **Tensões cosmológicas:** Di Valentino et al. (2021)

---

## ⚖️ Licença

Este trabalho está disponível sob licença MIT para fins acadêmicos e científicos.

---

**Última atualização:** 28 de Novembro de 2025  
**Autor:** Nil Silva  
**Contato:** [a ser adicionado]  
**Status:** Preparação para submissão ao arXiv
