# Summary of PyTorch

## Basics

### Creating tensors

```python
torch.arange(a) # tensor([0,1,...,a-1])
torch.arange(a,b) # tensor([a,a+1,...,b-1])
```

### Operations

```python
torch.dot(u,v) # dot product between u and v
```

## Autograd and Backprop
```python
# x is a tensor
x.requires_grad_(True) # register 'x' for autograd
x.grad # gradients of 'x', if computed with backward
x_.grad.zero_() # resets the gradient
```

```python
y.backward() # computes the backprop on 'y' and evaluates gradients
```