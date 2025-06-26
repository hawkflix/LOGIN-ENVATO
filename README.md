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
    <div className="p-4 max-w-4xl mx-auto">
      <h1 className="text-3xl font-bold mb-4">Organizador de Projetos</h1>

      <div className="grid gap-4 mb-6">
        <Input
          placeholder="Nome do Projeto"
          value={title}
          onChange={(e) => setTitle(e.target.value)}
        />
        <Textarea
          placeholder="Descrição do Projeto"
          value={description}
          onChange={(e) => setDescription(e.target.value)}
        />
        <select
          className="border rounded px-4 py-2"
          value={status}
          onChange={(e) => setStatus(e.target.value)}
        >
          <option value="Em andamento">Em andamento</option>
          <option value="Concluído">Concluído</option>
          <option value="Pendente">Pendente</option>
        </select>
        <Button onClick={addProject}>Adicionar Projeto</Button>
      </div>

      <div className="grid gap-4">
        {projects.map((project) => (
          <Card key={project.id}>
            <CardContent className="p-4">
              <h2 className="text-xl font-semibold">{project.title}</h2>
              <p className="text-sm text-gray-500 mb-2">{project.status}</p>
              <p>{project.description}</p>
            </CardContent>
          </Card>
        ))}
      </div>
    </div>
  );
}
