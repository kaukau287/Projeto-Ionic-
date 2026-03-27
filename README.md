# Projeto-Ionic-
Trabalho sobre mim como iniciei na programação

### `src/pages/Home.tsx`
```tsx
import { useNavigate } from "react-router-dom";
import profilePhoto from "@/assets/profile-photo.jpg";

const Home = () => {
  const navigate = useNavigate();

  return (

        Cartão de Identificação

          {/* Header band */}

          {/* Info */}

              Kauã de Araújo Pereira da Silva

                Matrícula: 25106415

                Unidade: Unisuam Augusto Motta

                Turno: Manhã

         navigate("/sobre")}
        >
          Sobre →

  );
};

export default Home;
```

### `src/pages/Sobre.tsx`
```tsx
import { useNavigate } from "react-router-dom";

const Sobre = () => {
  const navigate = useNavigate();

  return (

        Sobre

            Sobre Mim

            Me chamo Kauã de Araújo Pereira da Silva e comecei a faculdade de
            Análise e Desenvolvimento de Sistemas no ano passado. Desde então,
            venho aprendendo cada vez mais sobre o mundo da programação e
            descobrindo novas tecnologias a cada semestre.

            Atualmente estou estudando linguagens como Python, Java, JavaScript,
            entre outras. Também tenho explorado o desenvolvimento web e mobile,
            aprendendo a criar aplicações completas, desde o front-end até o
            back-end. Cada projeto é uma oportunidade de evoluir e aprimorar
            minhas habilidades.

            Meu objetivo é me tornar um desenvolvedor completo, capaz de
            resolver problemas reais através da tecnologia. Estou sempre em
            busca de novos desafios e conhecimentos que me ajudem a crescer
            profissionalmente na área de TI.

         navigate("/")}
        >
          ← Voltar ao Início

  );
};

export default Sobre;
```

### `src/App.tsx`
```tsx
import { Toaster } from "@/components/ui/toaster";
import { Toaster as Sonner } from "@/components/ui/sonner";
import { TooltipProvider } from "@/components/ui/tooltip";
import { QueryClient, QueryClientProvider } from "@tanstack/react-query";
import { BrowserRouter, Routes, Route } from "react-router-dom";
import Home from "./pages/Home";
import Sobre from "./pages/Sobre";
import NotFound from "./pages/NotFound";

const queryClient = new QueryClient();

const App = () => (

          } />
          } />
          } />

);

export default App;
```

### CSS customizado adicionado ao `src/index.css` (adicione ao final do arquivo):
```css
/* Ionic-inspired utility classes */
.ionic-page {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  background: hsl(var(--background));
}

.ionic-toolbar {
  padding: 1rem 1.25rem;
  font-size: 1.125rem;
  font-weight: 700;
  text-align: center;
  background: hsl(217 91% 60%);
  color: white;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.ionic-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 1.5rem 1rem;
}

.ionic-card {
  width: 100%;
  max-width: 24rem;
  border-radius: 1rem;
  background: hsl(var(--card));
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
  overflow: hidden;
}

.ionic-btn {
  padding: 0.75rem 1.5rem;
  border-radius: 0.75rem;
  font-weight: 600;
  font-size: 0.95rem;
  color: white;
  background: hsl(217 91% 60%);
  border: none;
  cursor: pointer;
  transition: opacity 0.2s;
}

.ionic-btn:hover {
  opacity: 0.9;
}

.ionic-btn-outline {
  padding: 0.75rem 1.5rem;
  border-radius: 0.75rem;
  font-weight: 600;
  font-size: 0.95rem;
  color: hsl(217 91% 60%);
  background: transparent;
  border: 2px solid hsl(217 91% 60%);
  cursor: pointer;
  transition: all 0.2s;
}

.ionic-btn-outline:hover {
  background: hsl(217 91% 60% / 0.1);
}
```




