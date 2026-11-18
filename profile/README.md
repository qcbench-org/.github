<p align="center">
  <img src="https://raw.githubusercontent.com/qcbench-org/qcbench/main/assets/avatar.png" alt="QCBench logo" width="160" height="160">
</p>

<h1 align="center">QCBench</h1>

<p align="center"><strong>Reproducible quantum computer characterization from experiments and shot counts.</strong></p>

<p align="center">
  <a href="https://pypi.org/project/qcbench/"><img src="https://img.shields.io/pypi/v/qcbench" alt="PyPI version"></a>
  <a href="https://github.com/qcbench-org/qcbench"><img src="https://img.shields.io/badge/source-GitHub-181717?logo=github" alt="Source repository"></a>
  <a href="https://github.com/qcbench-org/qcbench/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-Apache--2.0-blue" alt="Project license: Apache-2.0"></a>
</p>

## About

QCBench plans QPU experiments, exports circuits and analyzes shot counts with statistical uncertainty and execution provenance. The first release covers readout assignment error, GHZ fidelity, mirror-circuit survival, T1 and spin-echo T2.

面向量子计算真机的测评与表征，提供电路计划、counts 分析、统计误差和可追溯报告。

## Install

```bash
pip install qcbench

# Optional IBM Runtime integration
pip install 'qcbench[ibm]'
```

## Try it

```bash
qcbench list
qcbench demo --directory demo-results
qcbench plan --physical-qubits 0 1 --output plan.json
```

## Available today

- Five hardware characterization families, with 40 circuits in the default two-qubit plan.
- OpenQASM 3 export, optional Qiskit device compilation and explicit IBM Runtime submission/collection.
- Plan-bound datasets, uncertainty estimates, coherence-fit diagnostics and JSON/CSV reports.

The demo is explicitly synthetic and runs offline. Hardware submission requires explicit opt-in; no paid QPU validation or real-device ranking is claimed for this release.

## Start here

- **[Source repository](https://github.com/qcbench-org/qcbench)** — implementation, examples and contributions.
- **[Documentation and quick start](https://github.com/qcbench-org/qcbench#readme)** — APIs, commands and methodology.
- **[PyPI package](https://pypi.org/project/qcbench/)** — installation and release files.
- **[Issues and proposals](https://github.com/qcbench-org/qcbench/issues)** — bugs, new tasks and feature requests.

## Benchmark family

| Project | Focus | Package |
| --- | --- | --- |
| [LastExam](https://github.com/lastexam-org) | AI and agent task evaluation | [lastexam](https://pypi.org/project/lastexam/) |
| [SDKBench](https://github.com/sdkbench-org) | SDK performance and correctness | [sdkbench](https://pypi.org/project/sdkbench/) |
| [QCBench](https://github.com/qcbench-org) | Quantum computer hardware characterization | [qcbench](https://pypi.org/project/qcbench/) |
