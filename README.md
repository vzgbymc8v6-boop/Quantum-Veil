### What is it, What physics does it use, Who is it for:



QUANTUM-VEIL is an interactive educational game designed to make quantum networking and its real-world applications more accessible, engaging, and enjoyable.
Link to game:https://quantum-networking-h-5kwe.bolt.host/

Quantum networking is an emerging field that uses the principles of quantum mechanics to transmit quantum information and connect quantum devices. Although it has the potential to transform secure communication, distributed quantum computing, and quantum sensing, its underlying concepts can be difficult for beginners to understand through traditional textbooks or technical explanations alone.

QUANTUM-VEIL addresses this learning challenge by presenting quantum communication as an interactive mission. Instead of only reading about quantum phenomena, players can explore the ideas behind quantum-secure communication through gameplay, experimentation, and problem-solving.

The project combines scientific concepts with game-based learning to introduce players to the foundations of quantum key distribution (QKD), a family of communication protocols that uses quantum states to help two parties establish a shared secret key and detect certain forms of eavesdropping.

The ultimate goal is to bridge the gap between complex quantum theory and intuitive understanding, helping students, beginners, and curious learners develop an interest in quantum technologies without requiring an advanced background in physics.


### The details of the physical phenomena used:
The scientific foundation of QUANTUM-VEIL is quantum information science, particularly the use of quantum mechanics to communicate information securely.

To understand why quantum networking is different from ordinary networking, it helps to start with the fundamental physics.

## 2.1 Classical bits versus quantum bits


Classical bit:
A classical bit stores either 0 or 1. Computers encode, copy, and transmit these bits using electrical signals, light, or other physical systems.

Qubit:
A qubit can exist in a quantum superposition of two basis states. Its information may be encoded in a photon's polarization, among other physical properties.


Super position: A superposition is not simply a classical bit that is secretly both 0 and 1. It is a quantum state whose measurement outcomes depend on the measurement basis.

Why this matters for our game: quantum communication cannot always be treated like sending ordinary binary data. The quantum state itself carries information, and how that state is measured matters. 


## 2.2 Quantum measurement and disturbance

In classical communication, someone can often inspect or copy a signal without fundamentally changing the information it carries.

Quantum mechanics is different. Measuring a qubit in an incompatible basis can disturb its state and change the statistics of subsequent measurements.

For example, imagine that a sender prepares a photon in one of two polarization states, but an eavesdropper does not know which measurement basis the sender used. If the eavesdropper chooses the wrong basis, the measurement can disturb the photon. The receiver may then detect unexpected discrepancies.

This is one of the physical principles behind quantum key distribution.

The important nuance is that not every quantum measurement necessarily destroys or changes every state. The disturbance depends on the state and measurement being used.

## 2.3 Quantum key distribution (QKD)


Quantum key distribution is a method for allowing two parties—commonly called Alice and Bob—to establish a shared secret cryptographic key using quantum states and classical communication.

A potential eavesdropper is conventionally called Eve.

A simplified example is the BB84 protocol, one of the best-known QKD protocols:

Step 1 — Alice prepares quantum states

Alice encodes random bits into quantum states, choosing randomly between two measurement bases. In a polarization-based illustration, these might be rectilinear and diagonal polarization bases.

Step 2 — Quantum transmission

Alice sends the photons to Bob through a quantum channel. Eve may attempt to intercept them, but certain interception strategies introduce detectable errors.

Step 3 — Basis comparison

Bob independently chooses measurement bases. Alice and Bob then communicate over a classical channel to identify which rounds used matching bases. They discard the mismatched rounds.

Step 4 — Error checking and key generation

They compare a sample of the remaining results to estimate the error rate. If the channel passes security checks, they can use classical error correction and privacy amplification to produce a secure shared key. Otherwise, they abort.

The security of real QKD depends on the protocol, implementation, device behavior, and appropriate classical authentication, not merely on using photons. 



## 2.4 The no-cloning theorem

Quantum mechanics prohibits making a perfect copy of an arbitrary unknown quantum state. This is known as the no-cloning theorem.

This is important because a quantum communication system cannot simply copy every unknown qubit, as a classical network can copy data packets.

The theorem also helps explain why an eavesdropper cannot always make a flawless copy of a quantum signal and leave the original untouched. Combined with the measurement properties used by QKD protocols, it contributes to the possibility of detecting certain attacks.

However, no-cloning alone does not guarantee that every quantum communication system is secure. Real implementations must also account for hardware flaws, side channels, and other attack strategies. 



## 2.5 Quantum networking beyond QKD

Although QKD is the central theme suggested by your game's title, quantum networking has broader goals.

Quantum teleportation: transfers an unknown quantum state using shared entanglement and classical communication. It does not teleport matter or send information faster than light. 

Quantum repeaters: aim to extend quantum communication over long distances by distributing entanglement across multiple network links, helping address transmission losses. 

Distributed quantum computing: could allow separate quantum processors to share quantum resources.

Quantum sensing: connected quantum systems may support measurements across multiple locations. 



These applications make quantum networking an important area of research for future communication and computing infrastructure.

### Gameplay and educational approaches:

The educational design is based on experiential learning: players encounter a problem, explore the underlying concepts, and develop an intuitive understanding of why quantum communication behaves differently from classical communication.

Rather than requiring players to begin with equations or advanced quantum theory, the game provides an accessible entry point into a field that is often perceived as abstract or difficult.

QUANTUM-VEIL aims to demonstrate that quantum networking is not only a topic for physicists and engineers. It is a technology that can be explored through interactive experiences, making its principles more approachable for students, beginners, and the wider public.

### Final Notes:

1. The game itself is linked on this website: https://quantum-networking-h-5kwe.bolt.host
2. The BB84 simulation is run on Qollab, make sure to use one of the IBM models when running it
3. Demonstration video is here (it is a video on canva):https://canva.link/90w86u2442qaepm