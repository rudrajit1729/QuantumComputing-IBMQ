# QuantumComputing-IBMQ
My journey in Quantum Computing on an IBM Quantum Computer accessed through Cloud

# Warning
The subject matter of quantum physics in general is very advanced, complex, confusing, and complicated. I am not a quantum physics expert. Dare I suggest too, no one is a quantum physics expert, but there are people far more qualified than me to talk on the theories and physics side of things.

I will still outline some basics, but I highly encourage you to dive into the theory and conceptual side of quantum physics on your own. I am going to focus mainly on the programming and application side of things here.

That said, some basic foundation is required, so:

# What are quantum computers?
Quantum computers are machines that work with qubits (quantum bits) rather than regular bits.

# What's a qubit?
A regular bit is a transistor that registers either a high or low voltage, which corresponds to 1 or 0 respectively. Through advances in technology over the years, we have bits that are nearly the size of atoms, which is absolutely incredible.

A quantum bit is a 2-state quantum "device." Many things can be used as qubits, such as a photon's horizontal and vertical polarization, or the spin up or spin down of an electron. What this means for us as computer scientists is that a qubit can be a 0, 1, or both.

Because...

Qubits also have 2 other very important properties:

- Superposition - this is where a qubit is, while left unobserved, all of its possible states. Once observed, it will collapse into one of the possible states.Hope Schrodinger's cat is meowing somewhere in your brain.These qubits have probabilities of occurances in particular states just like any other quantum sized particles. There is a lot more including Heisenberg's Uncertainty Theorem and I strongly encourage delving through the theory for better understanding of my work.

- Entanglement - This is where one qubit's state is linked to another. When entangled with eachother, a change in one of the entangled qubits will change the other instanty. At any distance. Take take that both of those words are fully intended. Instantly and *any* distance, which is what Einstein referred to as "Spooky action at a distance," since this appeared to violate various rules like transmitting information faster than the speed of light. This is referred to as quantum non-locality. 

For showing quantum properties the quantum dots(generally leverages silicon for making a ring) must be under the following environmental conditions:

- Material should be in a vacuum room and should be free from all kinds of radiation.Even a slight noise can generate computational errors.

- The quantum dot should be at a very low temperature, ideally at absolute zero (0K).

# What problems are quantum computers for?
Quantum computers wont be replacing classical computers. They're more likely to continue working alongside them, just as they are already doing today. As you will see, we tend use a classical computer to represent a quantum circuit to the quantum computer, the quantum computer runs some cycles on this circuit, and then reports back to us again with a classical bit response.

Quantum computers work very well for problems that exponentially explode.

Problems like logistics, such as the most ideal delivery route for trucks, or even concepts like planning for companies, where each choice branches out into new possible choices and opportunities.

This might still seem vague. Let's consider you're planning a charity dinner and you're attempting to seat people together who will keep eachother in good, donating, moods.

Let's pretend for now you just have 1 table with 5 seats. How many combinations do we have here? Well, it's 5x4x3x2x1, or 5 factorial, which is 120. This means there are 120 possible combinations.

What happens if we added... just one more seat? That'd be 6 factorial, which gives us 6x5-factorial, or 720. Just one more seat is 6x as many combinations.

What about 10 seats? That's 3,628,800 combinations.

Modeling is probably the most near-term real-world example that I see quantum computers being useful.

Classical computers can barely simulate many single molecules...and they do a very poor job of it (due to the issue of how many possibilities there are given a situation). You currently cant rely on a classical computer to do chemistry simulations reliably.

A quantum computer can actually model many molecules already today reliably, and it only gets better from here seemingly.

How do quantum computers consider, fundamentally, more possibilities at once?
With classical computers:

n_states = 2 x n_bits

With quantum computers:

n_states = 2^n_bits

Being exponential like this gives us some phenomenal properties. This is why quantum computers can help us with heavy-optimization types of tasks, or just tasks that have many possibilities.

# Quantum computers are probability
I think the simplest explanation of a quantum computer that I can come up with for now is that:

Classical computers can approximate and synthesize probability, they are not truly accurate and can never be with most tasks that use probability, unless of course you really can fit the entire range of possibilities into memory. Then you can get pretty close. But again, the probability space tends to explode as you add more variables.

Quantum computers do not model probability. They simply are the probability.

For this reason, quantum computers are also great for modeling things like molecules. With quantum computers, we could perform many chemistry experiments solely on quantum computers, which should significantly speed up many areas of research.

# How to access a quantum computer?
We *can* access quantum computers in the cloud!
Google, Microsoft, IBM, D-Wave offer some form of cloud-based quantum computer access.

I found IBM's to be the easiest to get up and running with. You really can go from nothing to running on an actual quantum computer in a few minutes for free.

# Requisites:
Python3 is the base requirement.
Create a conda environment using *conda create --name Qiskit python=3.7*

Activate the conda environment using *conda activate Qiskit*

Then run *pip install qiskit numpy jupyterlab matplotlib qiskit-ibmq-provider* for the required packages.

Go to quantum_computing.ibm.com and generate your token. I did this project as a part of research work so got premium access but you can try a community edition.









