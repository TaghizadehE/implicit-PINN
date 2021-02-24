## [Implicit-physics-informed neural networks for nonlinear closure: The case of transport in tissues](https://github.com/TaghizadehE/implicit-PINN)

data-driven machine learning for explicitly closing nonlinear problems during upscaling

<img src="https://render.githubusercontent.com/render/math?math=\frac{\partial c_{\sigma}}{\partial t}">

\begin{align}
\intertext{\it Mass: Extracellular phase}
&&    \frac{\partial c_{\beta}}{\partial t} = -{\bf v}_\beta \nabla \cdot c_{\beta} &+\nabla\cdot(\mathscr{D}_{\beta}\nabla c_{\beta})
\label{microe}\\
%
%\intertext{\it Boundary conditions}
&B.C.~1& -{\bf n}_{\beta\sigma} \cdot \mathscr{D}_{\beta} \nabla c_{\beta} &= -{\bf n}_{\beta\sigma} \cdot \mathscr{D}_{\sigma} \nabla c_{\sigma},\nonumber \\
&&&~\textrm{at cell surface}\\
&B.C.~2& c_{\beta} = & c_{\sigma},~\textrm{at cell surface}\\
&I.C.1& c_{\beta}({\bf x},0)& =\mathscr{I}_\beta({\bf x})\\
%
\intertext{\it Mass: Intracellular phase}
&&\frac{\partial c_{\sigma}}{\partial t} =  \nabla\cdot(\mathscr{D}_{\sigma}\nabla c_{\sigma})& -k_m \frac{c_{\sigma}}{c_{\sigma}+K} \label{nonlin} \\
&I.C.~2& c_{\sigma}({\bf x},0)& =\mathscr{I}_\sigma({\bf x})
\label{microi}
%
\end{align}
