# 1823. Find the winner of the Circular Game

$$
\usetikzlibrary {arrows.meta, backgrounds}
\begin{tikzpicture} [background rectangle/.style={fill=white}, show background rectangle]
    \def \n {5}
    \def \radius {3}
    \def \margin {8}
    \foreach \i in {1,...,\n} {
        \node[draw, circle] (\i) at ({360 / \n * (\i - 1)}:\radius) {\i};
        \draw[-Stealth] ({360 / \n * (\i - 1) + \margin}:\radius) arc ({360 / \n * (\i - 1) + \margin}:{360 / \n * \i - \margin}:\radius);
    }
\end{tikzpicture}
$$
