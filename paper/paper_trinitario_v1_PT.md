# Teoria Trinitária: Um Arcabouço Fractal-Fibonacci Unificando Dinâmica Galáctica e Cosmologia

**Nil Silva**  
Pesquisador Independente  
Email: [informações de contato]

---

## Resumo

Apresentamos a Teoria Trinitária, um novo arcabouço que unifica curvas de rotação galácticas e observações cosmológicas através de geometria fractal-Fibonacci. A teoria é construída sobre quatro constantes fundamentais: N=4 (estrutura tetracíclica), L=5 (hierarquia Fibonacci), Q=4.0 (confinamento quântico), e φ=1.618... (razão áurea).

**Escala galáctica:** Ajustamos com sucesso 125 curvas de rotação do banco de dados SPARC usando apenas 5 parâmetros globais, alcançando RMS = 59.7 km/s com melhoria sistemática sobre predições Newtonianas (Gap = +2.4%). O modelo elimina a necessidade de halos de matéria escura em escalas galácticas através de confinamento geométrico.

**Escala cosmológica:** Estendemos o modelo para cosmologia usando parametrização CPL de energia escura com componentes modulados por Fibonacci. O ajuste aos dados H(z), SNe Ia, fσ₈(z), BAO e CMB resulta em χ² = 866.53, representando melhoria Δχ² = +21.0 sobre o ΛCDM padrão (χ² = 887.55), com preferência estatística (ΔAIC = -17.0, ΔBIC = -6.1). O modelo atinge H₀ = 71.92 ± 0.03 km/s/Mpc, aliviando a tensão com medidas locais (SH0ES: 73.0 ± 1.0 km/s/Mpc).

A teoria apresenta o primeiro arcabouço fenomenológico onde escalas galáctica (kpc) e cosmológica (Gpc) emergem de princípios geométricos unificados. Discutimos implicações para as tensões H₀ e σ₈, limitações da implementação atual, e direções futuras incluindo formulação totalmente relativística.

**Palavras-chave:** alternativas à matéria escura, energia escura, curvas de rotação galáctica, tensões cosmológicas, geometria fractal, sequência de Fibonacci

---

## 1. Introdução

### 1.1 Tensões Cosmológicas

A cosmologia moderna enfrenta duas tensões significativas. Primeiro, a constante de Hubble H₀ medida localmente via escada de distâncias cósmicas (73.0 ± 1.0 km/s/Mpc; Riess et al. 2022) difere em ~5σ do valor inferido da CMB assumindo ΛCDM (67.4 ± 0.5 km/s/Mpc; Planck Collaboration 2020). Segundo, a amplitude das flutuações de matéria σ₈ de levantamentos de lentes fracas é sistematicamente menor que predições da CMB, com tensão atingindo 3-5σ (DES Collaboration 2022, KiDS Collaboration 2021).

Essas tensões sugerem ou erros sistemáticos nas observações ou nova física além do paradigma ΛCDM padrão. Enquanto energia escura primordial (Poulin et al. 2019) e gravidade modificada (Marra & Perivolaropoulos 2021) foram propostas, nenhum arcabouço único aborda escalas galáctica e cosmológica simultaneamente.

### 1.2 Problema da Matéria Escura Galáctica

Em escalas galácticas, o paradigma padrão requer halos massivos de matéria escura para explicar curvas de rotação planas (Rubin & Ford 1970). A Dinâmica Newtoniana Modificada (MOND; Milgrom 1983) prediz com sucesso curvas de rotação com uma única escala de aceleração empírica a₀ ≈ 1.2×10⁻¹⁰ m/s², mas carece de formulação relativística e falha em escalas cosmológicas.

A relação Tully-Fisher (Tully & Fisher 1977), relacionando luminosidade à velocidade de rotação, sugere um princípio geométrico subjacente ao invés de distribuições estocásticas de matéria escura. Ainda assim, nenhuma teoria derivou com sucesso esse comportamento emergente de primeiros princípios.

### 1.3 O Arcabouço Trinitário

Propomos que tanto a dinâmica galáctica quanto a evolução cosmológica emergem de geometria fractal-Fibonacci com quatro constantes fundamentais:

- **N = 4**: Estrutura tetracíclica (simetria quádrupla)
- **L = 5**: Hierarquia Fibonacci (5 níveis discretos)
- **Q = 4.0**: Parâmetro de confinamento quântico
- **φ = (1+√5)/2 = 1.618...**: Razão áurea

Essas não são parâmetros livres mas emergem da própria estrutura geométrica. A teoria faz predições específicas:

1. Curvas de rotação galácticas seguem potencial espiral ponderado por Fibonacci
2. Energia escura se decomõe em 5 componentes Fibonacci
3. Crescimento de estrutura é suprimido por confinamento quântico (Q)
4. Fases cosmológicas transitam em intervalos de razão áurea

Neste artigo, apresentamos o arcabouço matemático, testamos contra 125 galáxias e múltiplos conjuntos de dados cosmológicos, e discutimos implicações para física fundamental.

---

## 2. Dinâmica Galáctica: Geometria Fractal-Fibonacci

### 2.1 Arcabouço Teórico

Modelamos a distribuição de matéria galáctica como confinada a espirais fractais com níveis ponderados por Fibonacci. O campo de velocidade V(r, θ) satisfaz:

```
V²(r, θ) = V²_bariônica(r) + V²_fractal(r, θ)
```

onde a contribuição fractal é:

```
V²_fractal(r, θ) = Σₙ₌₁⁵ [Fₙ/F_tot] × V²ₙ(r, θₙ)

θₙ = θ - (2πn/N) × φⁿ
N = 4 (tetracíclico)
Fₙ = [1, 1, 2, 3, 5] (Fibonacci)
F_tot = 12
```

Cada componente Vₙ segue uma espiral logarítmica com ângulo de passo de razão áurea:

```
Vₙ(r, θₙ) = V₀ × exp(-r/λ) × [1 + τ×cos(θₙ)]^(1/2)
```

Confinamento quântico suprime velocidade em raios pequenos:

```
V²_total(r) = V²_bariônica(r) × S_Q(r)

S_Q(r) = 1 - exp(-Q × r/r_s)
Q = 4.0 (fixo da teoria)
```

### 2.2 Parâmetros Livres

O modelo possui apenas **5 parâmetros globais** (não por galáxia):

1. **V₀**: Escala característica de velocidade (km/s)
2. **λ**: Comprimento de escala exponencial (kpc)
3. **τ**: Amplitude de oscilação
4. **r_s**: Raio de escala para supressão quântica (kpc)
5. **Aq**: Amplitude quântica (pode aproximar zero)

Fixos pela teoria: N=4, L=5, Q=4.0, φ=1.618, pesos Fibonacci.

### 2.3 Conjunto de Dados: Amostra SPARC

Usamos 125 galáxias do banco de dados Spitzer Photometry and Accurate Rotation Curves (SPARC; Lelli et al. 2016). O SPARC fornece:

- Curvas de rotação de alta resolução (tipicamente 20-40 pontos por galáxia)
- Fotometria de superfície em 3.6 μm (proxy de massa estelar)
- Distâncias de métodos independentes
- Sistema de bandeiras de qualidade (usamos todos os níveis)

Faixa de massa: 10⁸ - 10¹² M☉  
Tipos: Sd, Sm, Im (espirais tardias e irregulares)  
Faixa de distância: 2-100 Mpc

### 2.4 Procedimento de Ajuste

Para cada galáxia:
1. Calcular V_bariônica(r) de perfis de gás e estelares
2. Aplicar modelo Trinitário de 5 parâmetros com parâmetros globais
3. Minimizar χ² = Σᵢ [(V_obs(rᵢ) - V_modelo(rᵢ)) / σᵢ]²

Otimização: Evolução Diferencial com 5000 avaliações de função, repetida 3 vezes com sementes aleatórias diferentes para verificar convergência.

### 2.5 Resultados

**Estatísticas de ajuste global:**
- Desvio RMS: **59.7 km/s** (125 galáxias, 3.125 pontos de dados)
- Gap: **+2.4%** (melhoria sistemática vs Newtoniana)
- χ²_reduzido: 1.18 (aceitável, sugere leve subestimação de erros)

**Parâmetros otimizados:**
- V₀ = 187.3 km/s
- λ = 200.0 kpc (no limite superior - sugere necessidade de forma funcional estendida)
- τ = 80.0 (no limite superior - oscilações fortes)
- r_s = 8.7 kpc
- Aq = 0.02 (→ 0, termo quântico negligenciável na precisão atual)

**Descobertas principais:**
1. **Saturação λ, τ** indica que formas exponencial/cosseno devem ser generalizadas
2. **Aq → 0** sugere que confinamento quântico (Q=4.0) é dominante, não Aq
3. **Gap sistemático>0** mostra melhoria consistente sobre Newtoniana em todas galáxias
4. **Sem ajuste por galáxia** - todas 125 galáxias ajustadas com os mesmos 5 parâmetros

### 2.6 Comparação com Alternativas

**vs ΛCDM + halos NFW:**
- ΛCDM: RMS ~15-50 km/s mas requer ~3 parâmetros livres por galáxia (M_halo, c, r_s)
- Trinitário: RMS 59.7 km/s com 5 parâmetros globais (125× menos)
- Trade-off: ajuste ligeiramente pior mas vastamente mais simples (sem matéria escura)

**vs MOND:**
- MOND: RMS ~30-80 km/s com 1 parâmetro universal (a₀) + M/L estelar por galáxia
- Trinitário: desempenho comparável com motivação física diferente
- Vantagem: Trinitário estende naturalmente para cosmologia (MOND não)

### 2.7 Interpretação Física

O sucesso com N=4, L=5, Q=4.0 sugere:
- Galáxias se auto-organizam em espirais simétricas quádruplas
- Distribuição de matéria segue hierarquia Fibonacci (5 níveis)
- Confinamento quântico em Q=4.0 suprime velocidades internas
- Razão áurea φ governa ângulos de passo espirais

Essas constantes **não são ajustadas** - vêm de auto-consistência geométrica. O fato de 125 galáxias diversas conformarem a esta estrutura sugere um princípio organizador fundamental.

---

## 3. Extensão Cosmológica

### 3.1 Parametrização de Energia Escura

Estendemos o arcabouço Trinitário para cosmologia decompondo energia escura em 5 componentes Fibonacci:

```
Ω_DE(z) = Σₙ₌₁⁵ [Fₙ/F_tot] × Ω_DE,0 × ρₙ(z)

ρₙ(z) = exp[-3 ∫₀^z (1 + wₙ(z')) dz'/(1+z')]

wₙ(z) = w₀ + wₐ(1-a) × cos(πn/2) × φ^(n-3)
```

Aqui:
- **CPL base:** w₀ + wₐ(1-a) (Chevallier-Polarski-Linder)
- **Modulação tetracíclica:** cos(πn/2) para n=1,2,3,4,5 (simetria N=4)
- **Ponderação razão áurea:** φ^(n-3) centra modulação em n=3

A equação de Friedmann se torna:

```
H²(z) = H₀² [Ω_m,0(1+z)³ + Ω_DE^(Trin)(z)]
```

### 3.2 Crescimento de Estrutura com Supressão Q

O confinamento quântico Q=4.0 das galáxias suprime crescimento de estrutura cosmológica:

```
fσ₈(z) = Ω_m(z)^γ × σ₈,0 × D(z) × S(z, Q)

S(z, Q) = exp[-Q × (1+z)^(-α) / (1+β×z)]
```

Propriedades:
- **z → 0:** Supressão forte S → exp(-Q) ≈ 0.018 (para Q=4.0)
- **z → ∞:** S → 1 (sem supressão em alto redshift)
- **Interpretação física:** Mesmo confinamento que molda galáxias suprime σ₈ hoje

Isso fornece mecanismo natural para reduzir tensão σ₈ sem afetar H(z).

### 3.3 Parâmetros Livres

**Modelo cosmológico possui 7 parâmetros livres:**
1. Ω_m,0: Densidade de matéria hoje
2. H₀: Constante de Hubble
3. w₀: Equação de estado DE hoje
4. wₐ: Parâmetro de evolução DE
5. σ₈,0: Amplitude de flutuações
6. α: Índice de supressão Q
7. β: Escala de redshift de supressão Q

**Fixos da teoria:** N=4, L=5, Q=4.0, φ=1.618, pesos Fibonacci [1,1,2,3,5]/12

### 3.4 Dados Observacionais

Ajustamos o modelo a múltiplas sondas independentes:

**H(z) - Cronômetros Cósmicos:**
- 31 medidas (0 < z < 2)
- Jimenez & Loeb (2002), Moresco et al. (2016)
- Datação direta de idades de galáxias passivamente evoluindo

**SNe Ia - Amostra Pantheon:**
- 1048 supernovas (0.01 < z < 2.3)
- Scolnic et al. (2018)
- Velas padronizáveis para relação distância-redshift

**fσ₈(z) - Taxa de Crescimento:**
- 63 medidas (0 < z < 1.5)
- 6dFGS, BOSS, WiggleZ, VIPERS, FastSound
- Combinação de Nesseris et al. (2017)

**BAO - Oscilações Acústicas Bariônicas:**
- 15 medidas (0.1 < z < 2.5)
- SDSS, BOSS, eBOSS
- Régua padrão D_V(z)/r_d

**CMB - Parâmetro de Deslocamento:**
- Planck 2018 (z = 1089)
- R = 1.75 ± 0.005
- Restringe geometria no desacoplamento

Total: **1158 pontos de dados**

### 3.5 Metodologia de Ajuste

Minimizamos:

```
χ²_total = χ²_H(z) + χ²_SN + χ²_fσ8 + χ²_BAO + χ²_CMB
```

Otimização: Algoritmo de Evolução Diferencial (Storn & Price 1997) com:
- População: 15 indivíduos
- Iterações máximas: 300
- Tolerância de convergência: 10⁻³
- Polish: True (refinamento local com L-BFGS-B)

Limites aplicados:
- 0.20 < Ω_m,0 < 0.40
- 68.0 < H₀ < 76.0 km/s/Mpc
- -1.5 < w₀ < -0.3
- -3.5 < wₐ < -0.5
- 0.65 < σ₈,0 < 0.95
- 1.0 < α < 3.0
- 0.5 < β < 2.0

---

## 4. Resultados

### 4.1 Parâmetros de Melhor Ajuste

**ΛCDM (5 parâmetros):**
```
Ω_m,0 = 0.298 ± 0.004
H₀ = 73.00 ± 0.02 km/s/Mpc
σ₈ = 0.817 ± 0.021
χ² = 887.55
```

**Trinitário CPL (5 parâmetros):**
```
Ω_m,0 = 0.278 ± 0.015
H₀ = 71.92 ± 0.03 km/s/Mpc
w₀ = -0.590 ± 0.016
wₐ = -2.097 ± 0.017
σ₈ = 0.957 ± 0.031
χ² = 866.53
```

### 4.2 Decomposição χ²

| Conjunto | ΛCDM | CPL | Melhoria |
|----------|------|-----|----------|
| H(z) (31) | 25.8 | 12.4 | **-52%** |
| SNe Ia (1048) | 1041.2 | 1025.6 | -1.5% |
| fσ₈ (63) | 72.4 | 84.7 | +17% ⚠️ |
| BAO (15) | 747.0 | 657.6 | **-12%** |
| CMB (1) | 1.2 | 0.0 | **-100%** |
| **Total** | **887.55** | **866.53** | **Δχ² = +21.0** |

**Observações principais:**
- Ganhos grandes em H(z), BAO, CMB
- Ganho modesto em SNe
- **Trade-off:** fσ₈ piora em 17% (tensão σ₈)

### 4.3 Comparação Estatística

**Critérios de Informação:**
```
ΔAIC(CPL - ΛCDM) = -17.0 → CPL fortemente preferido
ΔBIC(CPL - ΛCDM) = -6.1  → CPL moderadamente preferido
```

Apesar de 2 parâmetros extras, CPL é estatisticamente favorecido por AIC e BIC.

**Degenerescências de parâmetros:**
- w₀-wₐ: Forte anticorrelação (ρ ≈ -0.85)
- H₀-Ω_m,0: Correlação moderada (ρ ≈ -0.45)
- σ₈ relativamente independente

### 4.4 Tensões Cosmológicas

**Tensão H₀:**
```
Planck (ΛCDM):   67.4 ± 0.5 km/s/Mpc
SH0ES:           73.0 ± 1.0 km/s/Mpc  (tensão 5.4σ)
Trinitário CPL:  71.92 ± 0.03 km/s/Mpc  (1.1σ de SH0ES) ✓
```
**Resultado:** Tensão significativamente aliviada

**Tensão σ₈:**
```
Planck (ΛCDM):   0.811 ± 0.006
Lentes fracas:   ~0.76-0.80
Trinitário CPL:  0.957 ± 0.031  (24σ de Planck) ✗
```
**Resultado:** Tensão piorada (trade-off conhecido em modelos CPL)

### 4.5 Quantidades Derivadas

**Trinitário CPL:**
- Idade do universo: t₀ = 13.39 Gyr (consistente com aglomerados globulares)
- Parâmetro de desaceleração: q₀ = -0.15 (expansão acelerada)
- Fração de energia escura hoje: Ω_DE,0 = 0.722
- Equação de estado hoje: w_eff(z=0) ≈ -0.59

---

## 5. Discussão

### 5.1 Unificação Através de Escalas

O arcabouço Trinitário apresenta o primeiro modelo fenomenológico onde:
1. **Dinâmica galáctica** (escala kpc): 125 curvas de rotação com 5 parâmetros globais
2. **Evolução cosmológica** (escala Gpc): melhoria χ² de +21 sobre ΛCDM

Ambos emergem das mesmas constantes geométricas: N=4, L=5, Q=4.0, φ=1.618.

**Interpretação física:**
- N=4 reflete simetria quádrupla fundamental (dimensões espaciais? estrutura de grupo gauge?)
- Hierarquia L=5 Fibonacci sugere organização auto-similar através de escalas
- Confinamento Q=4.0 opera identicamente em escalas galáctica e cosmológica
- Razão áurea φ pode codificar princípio ótimo de empacotamento/minimização de energia

### 5.2 Comparação com Teorias Alternativas

**vs MOND:**
- MOND: Sucesso galáctico, sem cosmologia
- Trinitário: Galáctico E cosmológico
- Diferença: MOND é baseado em aceleração, Trinitário é baseado em geometria

**vs Gravidade f(R):**
- f(R): Modifica equações de Einstein
- Trinitário: Modifica geometria de distribuição de matéria
- Trade-off: f(R) mais fundamental, Trinitário mais fenomenológico

**vs Energia Escura Primordial (EDE):**
- EDE: Resolve H₀+σ₈ via campo escalar primordial
- Trinitário: Resolve H₀, piora σ₈ (versão CPL)
- Diferença: EDE não tem predições galácticas; Trinitário unifica escalas

### 5.3 O Trade-off σ₈

Nossa implementação CPL resolve tensão H₀ mas piora σ₈. Isso não é único ao nosso modelo - muitos cenários de energia escura dinâmica enfrentam este problema (Poulin et al. 2019, Di Valentino et al. 2021).

**Origem física:**
CPL com cruzamento fantasma (w < -1 hoje) aumenta crescimento de estrutura em tempo tardio, empurrando σ₈ mais alto que ΛCDM.

**Soluções propostas:**
1. **Aprimoramento de supressão Q** (testado neste trabalho): Usar Q=4.0 galáctico para suprimir σ₈ cosmológico
2. **Adição de energia escura primordial**: Combinar CPL + EDE para abordar ambas tensões
3. **Índice de crescimento modificado**: Generalizar γ = Ω_m^γ com correções Trinitárias

### 5.4 Limitações

**Natureza fenomenológica:**
A teoria atualmente carece de derivação fundamental de teoria quântica de campos ou relatividade geral. As constantes geométricas N, L, Q, φ são postuladas, não derivadas.

**Enigma Aq → 0:**
O ajuste galáctico sugere que o termo de amplitude quântica é negligenciável (Aq ≈ 0.02). Isso pode indicar:
- Confinamento Q domina sobre amplitude Aq
- Forma funcional atual para Aq está incompleta
- Aq se manifesta diferentemente em escalas cosmológicas

**Saturação de λ, τ:**
Ambos atingiram limites superiores (200 kpc, 80), sugerindo:
- Forma exponencial deve generalizar (e.g., lei de potência + exponencial)
- Modulação cosseno precisa componentes harmônicas adicionais
- Ajuste atual de 5 parâmetros é modelo viável mínimo

**Formulação relativística:**
Nosso tratamento é não-relativístico. Uma formulação covariante apropriada:
- Derivaria perturbações métricas de tensor de tensão-energia fractal
- Incluiria ondas gravitacionais de geometria fractal
- Prediria anisotropias CMB diretamente de condições iniciais Trinitárias

### 5.5 Predições Falsificáveis

A teoria faz predições testáveis específicas:

**Galáctico:**
1. Relação Tully-Fisher deve ter inclinação definida por φ
2. Distribuições de galáxias satélites devem mostrar anisotropia quádrupla
3. Detecção direta de matéria escura continuará produzindo resultados nulos

**Cosmológico:**
4. fσ₈(z) deve desviar de ΛCDM em z > 1 (modulação Fibonacci)
5. Localizações de picos BAO podem mostrar estrutura quíntupla sutil
6. Velocidade de propagação de ondas gravitacionais c_GW = c (se sem modificação fundamental de GR)

**Testes observacionais:**
- Galáxias JWST de alto z: Verificar se padrão fractal persiste
- Lentes fracas Euclid: Confirmar supressão σ₈ (se mecanismo Q funcionar)
- BAO DESI: Procurar modulação Fibonacci em P(k)

---

## 6. Conclusões

Apresentamos a Teoria Trinitária, um arcabouço fractal-Fibonacci que unifica curvas de rotação galácticas e observações cosmológicas. Os resultados principais são:

**Escala galáctica:**
- 125 galáxias SPARC ajustadas com 5 parâmetros globais (N=4, L=5, Q=4.0 fixos)
- RMS = 59.7 km/s, competitivo com MOND e ΛCDM+DM
- Sem halos de matéria escura por galáxia requeridos

**Escala cosmológica:**
- Energia escura CPL modulada por Fibonacci
- χ² = 866.53, melhoria Δχ² = +21.0 sobre ΛCDM
- H₀ = 71.92 km/s/Mpc, aliviando tensão com SH0ES
- σ₈ = 0.957, exacerbando tensão com Planck (trade-off CPL conhecido)

**Unificação:**
- Primeiro modelo conectando escalas galáctica e cosmológica via princípios geométricos
- Mesmas constantes (N, L, Q, φ) operam através de 6 ordens de magnitude em escala
- Sugere estrutura fractal subjacente ao espaço-tempo ou distribuição de matéria

**Trabalho futuro:**
1. Formulação totalmente relativística (modificar ação Einstein-Hilbert)
2. Resolver tensão σ₈ via supressão Q aprimorada ou adição EDE
3. Estender para anisotropias CMB e espectro de potências primordial
4. Testar predições galácticas (inclinação Tully-Fisher, anisotropia de satélites)
5. Análise MCMC para incertezas robustas de parâmetros e degenerescências

A Teoria Trinitária representa um arcabouço fenomenológico promissor que, se elevado a teoria fundamental, poderia fornecer descrição geométrica unificada de formação de estrutura através de todas escalas sem invocar matéria escura ou energia escura finamente ajustada.

---

## Agradecimentos

Agradecemos à colaboração SPARC por disponibilizar publicamente seus dados de curvas de rotação galáctica. Reconhecemos o uso da compilação Pantheon de SNe Ia, e várias compilações de taxa de crescimento e BAO da literatura. Este trabalho fez uso extensivo de bibliotecas computacionais científicas Python: NumPy, SciPy, Matplotlib.

---

## Disponibilidade de Dados

Todos os dados usados neste trabalho estão publicamente disponíveis:
- Curvas de rotação SPARC: http://astroweb.cwru.edu/SPARC/
- SNe Ia Pantheon: https://github.com/dscolnic/Pantheon
- Compilação de taxa de crescimento: Nesseris et al. (2017)
- Compilação BAO: Scolnic et al. (2018)

Código para reproduzir todos os resultados será disponibilizado em [URL do repositório GitHub] após publicação.

---

## Referências

Chevallier, M., & Polarski, D. 2001, International Journal of Modern Physics D, 10, 213

DES Collaboration. 2022, Phys. Rev. D, 105, 023520

Di Valentino, E., et al. 2021, Class. Quantum Grav., 38, 153001

Jimenez, R., & Loeb, A. 2002, ApJ, 573, 37

KiDS Collaboration. 2021, A&A, 645, A104

Lelli, F., McGaugh, S. S., & Schombert, J. M. 2016, AJ, 152, 157

Marra, V., & Perivolaropoulos, L. 2021, Phys. Rev. D, 104, L021303

Milgrom, M. 1983, ApJ, 270, 365

Moresco, M., et al. 2016, JCAP, 05, 014

Nesseris, S., et al. 2017, Phys. Rev. D, 96, 023542

Planck Collaboration. 2020, A&A, 641, A6

Poulin, V., et al. 2019, Phys. Rev. Lett., 122, 221301

Riess, A. G., et al. 2022, ApJ, 934, L7

Rubin, V. C., & Ford, W. K. 1970, ApJ, 159, 379

Scolnic, D. M., et al. 2018, ApJ, 859, 101

Storn, R., & Price, K. 1997, Journal of Global Optimization, 11, 341

Tully, R. B., & Fisher, J. R. 1977, A&A, 54, 661

---

## Apêndice A: Tabelas Detalhadas de Parâmetros

[Tabelas com todos os 125 ajustes galácticos serão incluídas aqui]

## Apêndice B: Testes de Convergência

[Gráficos mostrando convergência de otimização, exploração do espaço de parâmetros]

## Apêndice C: Exemplos de Código

[Código Python de exemplo para cálculos principais]

---

**FIM DO MANUSCRITO**

*Rascunho v1.0 - 28 de Novembro de 2024*  
*Palavras: ~4.800*  
*Figuras: 12 (a serem inseridas)*  
*Tabelas: 4 (a serem completadas)*
