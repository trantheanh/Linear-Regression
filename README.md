# Linear Regression

This is a **very simple** Linear Regression implementation. I start from implement the algorithm from "for-loop" for only one feature to "vectorization" for n feature.

## Model:
\\[ \hat{y} = w_1 x_1 + w_2 x_2 + ... + w_n x_n + b\\]
\\[ \hat{Y} = W^T X + b \\]

$$ \documentclass{article}
\usepackage{amsmath}
\begin{document}
  \begin{align}
    W &= \begin{bmatrix}
           w_{1} \\
           w_{2} \\
           \vdots \\
           w_{n}
         \end{bmatrix}
  \end{align}
\end{document}
$$

## Loss function: 
\\[ \mathcal{L} (a) = \frac{1}{2m} \sum ^{m} _{i=1} (\hat{y} - y)^{2} \\]

## Loss function derivative (gradient, slope):
\\[ \mathcal{L}' (w_1) = \frac{\partial \mathcal{L}}{\partial w_1} = \frac{1}{m} \sum ^{m} _{i=1} (\hat{y} - y) x_1 \\] 
\\[ \mathcal{L}' (w_2) = \frac{\partial \mathcal{L}}{\partial w_2} = \frac{1}{m} \sum ^{m} _{i=1} (\hat{y} - y) x_2 \\] 
\\[ ... \\]
\\[ \mathcal{L}' (w_n) = \frac{\partial \mathcal{L}}{\partial w_n} = \frac{1}{m} \sum ^{m} _{i=1} (\hat{y} - y) x_n \\] 
\\[ \mathcal{L}' (b) = \frac{\partial \mathcal{L}}{\partial b} = \frac{1}{m} \sum ^{m} _{i=1} (\hat{y} - y) \\]

## Training set format:
Instead of calculate individual data point, we shape training set into a matrix to implement vectorization. Training set containt **m** data point which is represented by a matrix **X** with **m** row and each row is one data point with **n** feature.

\\[ x^{(1)}_1 \space \space \space x^{(1)}_2 \space \space \space x^{(1)}_3 \space \space \space ... \space \space \space x^{(1)}_n \\]
\\[ x^{(2)}_1 \space \space \space x^{(2)}_2 \space \space \space x^{(2)}_3 \space \space \space ... \space \space \space x^{(2)}_n \\]
\\[ x^{(3)}_1 \space \space \space x^{(3)}_2 \space \space \space x^{(3)}_3 \space \space \space ... \space \space \space x^{(3)}_n \\]
\\[ ... \\]
\\[ x^{(m)}_1 \space \space \space x^{(m)}_2 \space \space \space x^{(m)}_3 \space \space \space ... \space \space \space x^{(m)}_n \\]

