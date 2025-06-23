import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import { Tabs, TabsContent, TabsList, TabsTrigger } from "@/components/ui/tabs";

export default function MabhukuMarket() {
  return (
    <main className="min-h-screen bg-gray-100 p-6">
      <header className="mb-8">
        <h1 className="text-4xl font-bold text-center text-gray-800">
          Mabhuku Market
        </h1>
        <p className="text-center text-gray-600 text-lg mt-2">
          Publish, sell, and discover Zimbabwean stories.
        </p>
      </header>

      <Tabs defaultValue="marketplace" className="max-w-5xl mx-auto">
        <TabsList className="grid grid-cols-2 mb-6">
          <TabsTrigger value="marketplace">Marketplace</TabsTrigger>
          <TabsTrigger value="author">Author Panel</TabsTrigger>
        </TabsList>

        <TabsContent value="marketplace">
          <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
            {[1, 2, 3].map((i) => (
              <Card key={i}>
                <CardContent className="p-4">
                  <h2 className="text-xl font-semibold">Book Title {i}</h2>
                  <p className="text-sm text-gray-600 mt-1">Author Name</p>
                  <p className="mt-2">Brief description of the book...</p>
                  <Button className="mt-4 w-full">Buy Now - $3.99</Button>
                </CardContent>
              </Card>
            ))}
          </div>
        </TabsContent>

        <TabsContent value="author">
          <Card>
            <CardContent className="space-y-4 p-6">
              <h2 className="text-2xl font-semibold">Upload Your Book</h2>
              <Input placeholder="Book Title" />
              <Input placeholder="Author Name" />
              <Textarea placeholder="Brief Description" />
              <Input type="file" />
              <Input type="number" placeholder="Price (USD)" />
              <Button className="w-full">Submit Book</Button>
            </CardContent>
          </Card>
        </TabsContent>
      </Tabs>

      <footer className="mt-12 text-center text-gray-500">
        &copy; 2025 Mabhuku Market. Powered by Zimbabwean Writers.
      </footer>
    </main>
  );
}
