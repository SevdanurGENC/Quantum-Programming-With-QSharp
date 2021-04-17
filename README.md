# Quantum-Programming-With-QSharp
Introduction to Quantum Programming with Q #

## 1.Gün:
- Complex Arithmetic
- Linear Algebra
- The-Qubit
- Single Qubit Gates

## 2.Gün:
- Multi-Qubit Systems
- Multi-Qubit Gates
- Superposition
- Measurements

## 3.Gün:
- Random Number Generation
- Teleportation
- Superdense Coding

## 4.Gün:
- Introduction to Oracles
- Introduction to Grover's Algorithm


## Develop with Q# Jupyter Notebooks
```
conda create -n qsharp-env -c quantum-engineering qsharp notebook
conda activate qsharp-env
jupyter notebook
```

```qsharp
open Microsoft.Quantum.Intrinsic;

operation SampleQuantumRandomNumberGenerator() : Result {
    use q = Qubit(); // Allocate a qubit.
    H(q);            // Put the qubit to superposition. It now has a 50% chance of being 0 or 1.
    let r = M(q);    // Measure the qubit value.
    Reset(q);
    return r;
}

%simulate SampleQuantumRandomNumberGenerator 
```





