# Documentación de Pulse Journal

Este repositorio publica la documentación técnica y de uso de Pulse Journal mediante Mintlify.

La sección Codex cubre:

- contrato v4.1 y aislamiento por usuario;
- campos personalizados y presets;
- Sources, Perfiles y Simulaciones;
- tipos y shapes de campo;
- API REST y servidor MCP;
- territorios, fronteras, áreas y puntos.

## Vista previa local

Instala la CLI de Mintlify y ejecuta el sitio desde la raíz:

```bash
npm i -g mint
mint dev
```

La vista previa queda disponible normalmente en `http://localhost:3000`.

## Publicación

Mintlify despliega desde la rama `main`. Antes de publicar:

1. valida que `docs.json` incluya cada página nueva;
2. revisa enlaces internos y frontmatter;
3. confirma que las páginas distingan contrato vigente de trabajo previsto;
4. fusiona la rama documental en `main`.

## Fuentes de verdad

- Schema activo: `GET https://mcp.standatpd.com/api/codex/schema`
- Backend: ExtractorW
- Persistencia: Supabase con ownership y RLS por usuario
- Transporte MCP: `https://mcp.standatpd.com/mcp`
