# Linear Regression

# LINEAR REGRESSION - n Variable

## Model:
$$ \hat{y} = w_1 x_1 + w_2 x_2 + ... + w_n x_n + b$$

## Loss function: 
$$ \mathcal{L} (a) = \frac{1}{2m} \sum ^{m} _{i=1} (\hat{y} - y)^{2} $$

## Loss function derivative (gradient, slope):
$$ \mathcal{L}' (w_1) = \frac{\partial \mathcal{L}}{\partial w_1} = \frac{1}{m} \sum ^{m} _{i=1} (\hat{y} - y) x_1 $$ 
$$ \mathcal{L}' (w_2) = \frac{\partial \mathcal{L}}{\partial w_2} = \frac{1}{m} \sum ^{m} _{i=1} (\hat{y} - y) x_2 $$ 
$$ ... $$
$$ \mathcal{L}' (w_n) = \frac{\partial \mathcal{L}}{\partial w_n} = \frac{1}{m} \sum ^{m} _{i=1} (\hat{y} - y) x_n $$ 
$$ \mathcal{L}' (b) = \frac{\partial \mathcal{L}}{\partial b} = \frac{1}{m} \sum ^{m} _{i=1} (\hat{y} - y) $$

