# shadcn
npx shadcn@latest init --preset b6p4yRN9rE --template vite --pointer

npx shadcn@latest add 

jsconfig.jon
{
  "compilerOptions": {
    "paths": {
      "@/*": ["./src/*"]
    }
  }
}


vite
import { defineConfig } from "vite";
import react from "@vitejs/plugin-react";
import tailwindcss from "@tailwindcss/vite";
import { fileURLToPath, URL } from "node:url";

export default defineConfig({
  plugins: [react(), tailwindcss()],
  resolve: {
    alias: {
      "@": fileURLToPath(new URL("./src", import.meta.url)),
    },
  },
});
