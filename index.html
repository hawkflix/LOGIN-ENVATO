import { useState } from 'react';
import { Card, CardContent } from "@/components/ui/card";
import { Input } from "@/components/ui/input";
import { Button } from "@/components/ui/button";
import { Textarea } from "@/components/ui/textarea";

export default function Dashboard() {
  const [projects, setProjects] = useState([]);
  const [title, setTitle] = useState("");
  const [description, setDescription] = useState("");
  const [status, setStatus] = useState("Em andamento");

  const addProject = () => {
    if (title.trim() !== "") {
      const newProject = {
        id: Date.now(),
        title,
        description,
        status,
      };
      setProjects([newProject, ...projects]);
      setTitle("");
      setDescription("");
    }
  };

  return (
    <div className="min-h-screen bg-gradient-to-br from-black via-zinc-900 to-gray-900 text-white p-6">
      <h1 className="text-4xl font-bold mb-6 text-center drop-shadow-xl">🛠️ Painel de Projetos</h1>

      <div className="bg-zinc-800/60 backdrop-blur-md rounded-2xl shadow-2xl p-6 max-w-3xl mx-auto mb-10">
        <div className="grid gap-4">
          <Input
            className="bg-zinc-700 border-zinc-600 text-white placeholder:text-zinc-400"
            placeholder="Nome do Projeto"
            value={title}
            onChange={(e) => setTitle(e.target.value)}
          />
          <Textarea
            className="bg-zinc-700 border-zinc-600 text-white placeholder:text-zinc-400"
            placeholder="Descrição do Projeto"
            value={description}
            onChange={(e) => setDescription(e.target.value)}
          />
          <select
            className="bg-zinc-700 border-zinc-600 text-white rounded px-4 py-2"
            value={status}
            onChange={(e) => setStatus(e.target.value)}
          >
            <option value="Em andamento">Em andamento</option>
            <option value="Concluído">Concluído</option>
            <option value="Pendente">Pendente</option>
          </select>
          <Button className="bg-emerald-500 hover:bg-emerald-600 transition-colors" onClick={addProject}>Adicionar Projeto</Button>
        </div>
      </div>

      <div className="grid gap-6 max-w-4xl mx-auto">
        {projects.map((project) => (
          <Card key={project.id} className="bg-zinc-800 border-zinc-700 shadow-md hover:scale-[1.02] transition-transform">
            <CardContent className="p-5">
              <h2 className="text-2xl font-bold text-emerald-400 mb-1">{project.title}</h2>
              <p className="text-sm italic text-zinc-400 mb-2">Status: {project.status}</p>
              <p className="text-zinc-200 leading-relaxed">{project.description}</p>
            </CardContent>
          </Card>
        ))}
      </div>
    </div>
  );
}
