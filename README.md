import { Card, CardContent, CardHeader, CardTitle } from "@/components/ui/card"
import { Button } from "@/components/ui/button"
import Link from "next/link"

export default function Component() {
  return (
    <div className="min-h-screen bg-gray-100 flex items-center justify-center p-4">
      <Card className="w-full max-w-md">
        <CardHeader>
          <CardTitle className="text-2xl font-bold text-center">云顶工作室github官网测试</CardTitle>
        </CardHeader>
        <CardContent className="space-y-4">
          <Button asChild className="w-full">
            <Link href="https://www.google.com" target="_blank" rel="noopener noreferrer">
              访问 Google
            </Link>
          </Button>
          <Button asChild className="w-full" variant="outline">
            <Link href="https://www.github.com" target="_blank" rel="noopener noreferrer">
              访问 GitHub
            </Link>
          </Button>
          <Button asChild className="w-full" variant="secondary">
            <Link href="https://www.openai.com" target="_blank" rel="noopener noreferrer">
              访问 OpenAI
            </Link>
          </Button>
        </CardContent>
      </Card>
    </div>
  )
}
