---
layout: post
title: "Revisiting my Master’s Thesis: A reconstructed and guided edition"
date: 2026-02-13
categories: research archives
tags: [formal verification, dfs, bfs, acl2, gacela, program derivation]
---

Nearly two decades ago, I wrote a Master’s thesis on the formal verification of graph algorithms — specifically, Depth-First Search (DFS) and Breadth-First Search (BFS). 
The work explored how to specify these algorithms formally, derive correct implementations from their specifications, and verify them using mechanized tools: 
first through _GaCeLa_, an academic environment that integrates specification, program derivation, and proof obligation generation, and then through _[ACL2](https://www.cs.utexas.edu/~moore/acl2/)_, 
a theorem prover used to discharge the resulting proof obligations.

The original thesis was written in Spanish and typeset in LaTeX. The compiled PDF remains publicly available, along with the original _GaCeLa_ and _ACL2_ artifacts. 
However, the LaTeX source files themselves are no longer available.

This series presents a reconstructed, revisited, and translated edition of that thesis.

The text has been carefully recovered from the compiled PDF. For the purpose of this series, it is being structurally cleaned and translated into English. 
In some places, I clarify explanations, slightly modernize notation, and improve structure for readability. 
My intention is that the formal content and core arguments remain faithful to the original work.

Nevertheless, this is not a rewrite. It is a re-reading — with the benefit of time.

---

## Why revisit it now?

This thesis was not my first encounter with formal reasoning — it was my second. 
My first sustained exploration of formal methods took place during my Bachelor’s thesis (Sep 2003–Dec 2004), focused on program derivation by refinement: 
a prototype editor to derive correct programs from formal specifications in the framework of the refinement calculus as presented by Carroll Morgan, 
using a language inspired by Dijkstra’s Guarded Command Language as implemented in _GaCeLa_. 
A shorter version of that work was presented at [CLEI 2005](https://clei.org/en/proceedings-clei-en/) in Cali, Colombia, under the title *“Un Editor de Programas por Refinamiento.”*

The DFS/BFS thesis (Sep 2005–Feb 2007), *“[Verificación formal asistida por computador de algoritmos de búsqueda en profundidad y en amplitud](https://www.researchgate.net/publication/393004451_Verificacion_Formal_Asistida_por_Computador_de_Algoritmos_de_Busqueda_en_Profundidad_y_en_Amplitud),”* however, 
is the earliest project for which I still retain [the mechanized proof artifacts](https://www.researchgate.net/publication/393067301_Tesis_Maestria_W_Urribarri_defensa_programas_pruebaszip). 
In that sense, it represents the first _almost_ complete digital trace of my engagement with automated reasoning tools.

Revisiting it now is not merely an archival exercise. Over the years, my professional path has remained closely connected to formal reasoning, 
the trustworthiness of software systems, and tool confidence. 
Reading this work again, I recognize both the enthusiasm of a younger version of myself and the foundations of questions that still occupy me today.

---

## An educational intention

This reconstructed edition is not meant only as an archive.

It is also an attempt to make a complete, small-scale formal verification project accessible to:

- Undergraduate computer science students,
- Software engineers curious about formal methods,
- Readers intrigued by theorem provers but unsure where to begin.

Formal verification is often presented either in highly abstract mathematical texts or in advanced research papers. 
It can appear intimidating, detached, or inaccessible.

This series walks through an end-to-end example from specification → to derivation → to invariant discovery → to mechanized proof.

Along the way, I occasionally pause to explain concepts in more accessible terms and to reflect on what I would explain differently today.

---

## What this edition is — and is not

This edition:

- Preserves the original intellectual structure,
- Cleans and clarifies the exposition,
- Adds light educational notes,
- Includes occasional present-day commentary.

It does not:

- Rewrite the results,
- Retroactively optimize the proofs,
- Or pretend the work was written yesterday.

The Spanish PDF remains the primary historical artifact, and the formal proofs are preserved in their original _ACL2_ form. This version is a bridge between the original work and the perspective I hold today.

---

## Structure of the Series

Each chapter of the original thesis will appear as a separate post under *Research & Archives*.

Each post will include:

- A reconstructed and translated chapter,
- Short educational notes for newcomers,
- Occasional reflections from my present perspective.

We will begin with Chapter 1 in a later post.
