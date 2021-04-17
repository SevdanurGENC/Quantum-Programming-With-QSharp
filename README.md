# Quantum-Programming-With-QSharp
Introduction to Quantum Programming with Q #

![image](https://user-images.githubusercontent.com/5441882/115098833-f60e8b80-9f3a-11eb-985e-eeee6c73b52c.png)


## Day 1 :
- Complex Arithmetic
- Linear Algebra
- The-Qubit
- Single Qubit Gates

## Day 2 :
- Multi-Qubit Systems
- Multi-Qubit Gates
- Superposition
- Measurements

## Day 3 :
- Random Number Generation
- Teleportation
- Superdense Coding

## Day 4 :
- Introduction to Oracles
- Introduction to Grover's Algorithm


## Develop with Q# Jupyter Notebooks
```
conda create -n qsharp-env -c quantum-engineering qsharp notebook
conda activate qsharp-env
pip install pytest
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





