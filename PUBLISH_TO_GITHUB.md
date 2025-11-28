# Como Publicar no GitHub

Este repositório já está inicializado com Git e pronto para ser publicado no GitHub.

## Passo 1: Criar Repositório no GitHub

1. Acesse [github.com](https://github.com) e faça login
2. Clique no botão **"+"** no canto superior direito → **"New repository"**
3. Preencha os campos:
   - **Repository name**: `trinitarian-cosmology-cpl`
   - **Description**: `A Fractal-Fibonacci Framework Unifying Galactic Dynamics and Cosmology - CPL v1.0`
   - **Visibility**: 
     - ✅ **Public** (recomendado para publicação científica)
     - ou **Private** (se quiser manter privado inicialmente)
   - **NÃO marque**: "Initialize this repository with a README" (já temos um)
   - **License**: Escolha "MIT License" se desejar
4. Clique em **"Create repository"**

## Passo 2: Conectar Repositório Local ao GitHub

O GitHub mostrará instruções. Use estas:

```bash
# No terminal, dentro do diretório trinitarian-cosmology-cpl/
cd /Users/nilsilva/Desktop/trinitarian-cosmology-cpl

# Adicionar remote (substitua Hanksx pelo seu nome de usuário GitHub)
git remote add origin https://github.com/Hanksx/trinitarian-cosmology-cpl.git

# Renomear branch para 'main' se necessário
git branch -M main

# Push inicial
git push -u origin main
```

**Importante**: Substitua `Hanksx` pelo seu nome de usuário real do GitHub!

## Passo 3: Verificar Upload

Após o push, acesse:
```
https://github.com/Hanksx/trinitarian-cosmology-cpl
```

Você deve ver:
- ✅ README.md formatado como página principal
- ✅ 12 figuras na pasta `figures/`
- ✅ Papers completos na pasta `paper/`
- ✅ Resultados JSON na pasta `results/`
- ✅ Total: ~150 arquivos

## Passo 4: Configurações Recomendadas do Repositório

No GitHub, vá em **Settings** do repositório e configure:

### 4.1 Descrição e Topics
- **Description**: Adicione a descrição acima
- **Website**: Se tiver site/página pessoal
- **Topics**: Adicione tags para facilitar busca:
  ```
  cosmology, dark-energy, astrophysics, python, astronomy,
  dark-matter, fibonacci, fractal-geometry, cpl-parametrization
  ```

### 4.2 GitHub Pages (Opcional)
Se quiser hospedar os HTMLs:
1. Settings → Pages
2. Source: Deploy from a branch
3. Branch: `main`, folder: `/paper`
4. Save

O paper HTML ficará em:
```
https://Hanksx.github.io/trinitarian-cosmology-cpl/paper_EN_with_figures.html
```

### 4.3 Releases (Opcional mas Recomendado)
Para criar versão v1.0 oficial:
1. No repo, clique em **"Releases"** → **"Create a new release"**
2. Tag: `v1.0`
3. Title: `Trinitarian Cosmology CPL v1.0`
4. Description:
   ```markdown
   ## First Official Release
   
   Complete implementation of Trinitarian Theory CPL parametrization.
   
   ### Key Results
   - **Galactic**: 125 SPARC galaxies, RMS 59.7 km/s
   - **Cosmology**: χ²=866.53 (Δχ²=-21 vs ΛCDM)
   - **H₀**: 71.92 km/s/Mpc (alleviates tension)
   - **Evidence**: ΔAIC=-17.0 (strong), ΔBIC=-6.1 (positive)
   
   ### Assets
   - Complete manuscript (English + Portuguese)
   - 12 publication-quality figures
   - Python implementation
   - Pre-computed results (JSON)
   ```
5. Clique **"Publish release"**

## Passo 5: Atualizar README com Link Correto

Edite o README.md e substitua:
```
git clone https://github.com/yourusername/trinitarian-cosmology-cpl.git
```

Por:
```
git clone https://github.com/Hanksx/trinitarian-cosmology-cpl.git
```

Commit e push:
```bash
git add README.md
git commit -m "Update repository URL in README"
git push
```

## Passo 6: Adicionar DOI Zenodo (Opcional mas Recomendado)

Para citação científica:

1. Acesse [zenodo.org](https://zenodo.org)
2. Login com conta GitHub
3. Settings → GitHub → Flip switch para seu repositório
4. Crie release v1.0 no GitHub (Passo 4.3)
5. Zenodo automaticamente gerará DOI
6. Adicione badge do DOI ao README:
   ```markdown
   [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXX)
   ```

## Verificação Final

Checklist antes de tornar público:

- [ ] README.md está completo e correto
- [ ] Todas as figuras aparecem corretamente
- [ ] Papers HTML abrem sem erros
- [ ] LICENSE está presente (MIT)
- [ ] Não há dados sensíveis commitados
- [ ] URLs estão corretos (sem "yourusername")
- [ ] Email/contato atualizado no README

## Compartilhamento

Após publicação, compartilhe:

### Para comunidade científica:
- Twitter/X: Thread com principais resultados
- arXiv: Referencie o GitHub no paper
- ResearchGate: Adicione como projeto

### Links úteis:
```
Repositório:  https://github.com/Hanksx/trinitarian-cosmology-cpl
Figures PDF:  https://github.com/Hanksx/trinitarian-cosmology-cpl/blob/main/paper/Trinitarian_Cosmology_Figures.pdf
Paper HTML:   https://github.com/Hanksx/trinitarian-cosmology-cpl/blob/main/paper/paper_EN_with_figures.html
Results JSON: https://github.com/Hanksx/trinitarian-cosmology-cpl/blob/main/results/best_fit_parameters.json
```

---

**Pronto!** Seu trabalho científico está publicado e acessível para a comunidade global! 🚀

Para questões ou problemas, abra uma issue no repositório.
