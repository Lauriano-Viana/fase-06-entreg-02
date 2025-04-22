### Análise Crítica Comparativa dos Modelos: YOLOv5( entrega 1), YOLOv8( padrão ) e CNN
# 🧪 Avaliação Comparativa de Modelos: YOLOv5 vs YOLOv8 vs CNN

## ✅ 1. Facilidade de uso/integração

| Modelo     | Avaliação |
|------------|-----------|
| **YOLOv5** | Muito fácil de usar. A documentação é robusta, com ampla comunidade e muitos tutoriais. Fácil integração com projetos Python e aplicações em tempo real. |
| **YOLOv8** | Ainda mais amigável que o YOLOv5. Interface moderna (`ultralytics`), comandos simplificados e suporte nativo para exportação de modelos (ONNX, CoreML, etc). |
| **CNN**    | Menos amigável. Exige maior esforço de implementação, ajuste e integração. Necessita maior conhecimento técnico. |

**🏆 Vencedor: YOLOv8**

---

## ✅ 2. Precisão do modelo

| Modelo     | Precision (P) | Recall (R) | mAP50 | mAP50-95 | Observações |
|------------|---------------|------------|-------|----------|-------------|
| **YOLOv5** | 0.934         | 1.0        | 0.995 | 0.582    | Excelente precisão geral e equilíbrio entre classes. |
| **YOLOv8** | 0.848         | 0.988      | 0.970 | 0.655    | Melhor desempenho em mAP50-95. Classe *onça* com performance impecável. |
| **CNN**    | cobra: 0.00<br>onça: 0.47 | cobra: 0.00<br>onça: 1.00 | — | — | Falhou na classe *cobra*. Desempenho geral insatisfatório. |

**🏆 Vencedor: YOLOv8** (destaque em mAP50-95)

---

## ✅ 3. Tempo de treinamento/customização

| Modelo     | Tempo de Treinamento | Observações |
|------------|----------------------|-------------|
| **YOLOv5** | 0.033 horas (~2 min) | Muito rápido, eficiente. Ideal para ambientes com poucos recursos. |
| **YOLOv8** | 0.155 horas (~9 min) | Mais demorado, mas ainda aceitável. |
| **CNN**    | (não informado) | Geralmente exige mais tuning e ajustes manuais. |

**🏆 Vencedor: YOLOv5**

---

## ✅ 4. Tempo de inferência

| Modelo     | Tempo por imagem | Observações |
|------------|------------------|-------------|
| **YOLOv5** | ~8.96 img/s (estimado) | Rápido e leve, ideal para aplicações em tempo real. |
| **YOLOv8** | 23.8 ms/inferência | Um pouco mais pesado, mas ainda muito bom para tempo real. |
| **CNN**    | (não informado) | Depende muito da arquitetura; sem dados não é possível comparar. |

**🏆 Vencedor: YOLOv5**

---

## 📊 Resumo final

| Critério                         | Melhor Modelo |
|----------------------------------|---------------|
| Facilidade de uso/integração     | YOLOv8        |
| Precisão geral                   | YOLOv8 (mAP50-95) |
| Tempo de treinamento/customização | YOLOv5        |
| Tempo de inferência              | YOLOv5        |

---

## 🧠 Conclusão

- **YOLOv8** se destaca em precisão e usabilidade moderna, sendo ideal para aplicações que exigem robustez e qualidade em diversas condições.
- **YOLOv5** é mais leve, rápido e ainda extremamente eficaz — excelente para produção em tempo real e dispositivos com menos poder de processamento.
- A **CNN personalizada** teve desempenho muito abaixo do esperado, especialmente na detecção da classe *cobra*.

> **Recomendação**:  
> - Para aplicações em produção **com foco em velocidade**, escolha **YOLOv5**.  
> - Para **máxima precisão e usabilidade moderna**, vá de **YOLOv8**.

## Link para o colab
[ YOLOV8 ](https://colab.research.google.com/drive/1e1iQx1GwI-EyIEw8rxAd89LeBQhvOQ2M?usp=sharing)
[ REDE CNN ](https://colab.research.google.com/drive/1nnEa6P7ollxjedinAl2nxEYyOxYaXziK?usp=sharing)
