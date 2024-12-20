id: event-registration-form
name: Event Registration Form
type: tsx
content: |-
  import React, { useState } from 'react';
  import { Input } from "@/components/ui/input";
  import { Button } from "@/components/ui/button";
  import { Select, SelectContent, SelectItem, SelectTrigger, SelectValue } from "@/components/ui/select";
  import { Card, CardContent, CardHeader, CardTitle } from "@/components/ui/card";
  import { Label } from "@/components/ui/label";
  import { CheckCircle2 } from 'lucide-react';

  const RegistrationForm = () => {
    const [formState, setFormState] = useState({
      name: '',
      phone: '',
      email: '',
      dietary: '',
    });
    const [isSubmitted, setIsSubmitted] = useState(false);
    const [errors, setErrors] = useState({});

    const validateForm = () => {
      const newErrors = {};
      if (!formState.name) newErrors.name = '請輸入姓名';
      if (!formState.phone) newErrors.phone = '請輸入手機號碼';
      if (!formState.email) newErrors.email = '請輸入 Email';
      if (!formState.dietary) newErrors.dietary = '請選擇飲食習慣';
      
      setErrors(newErrors);
      return Object.keys(newErrors).length === 0;
    };

    const handleSubmit = (e) => {
      e.preventDefault();
      if (validateForm()) {
        setIsSubmitted(true);
      }
    };

    if (isSubmitted) {
      return (
        <Card className="w-full max-w-md mx-auto mt-10 p-6">
          <CardContent className="text-center">
            <CheckCircle2 className="w-16 h-16 text-green-500 mx-auto mb-4" />
            <h2 className="text-2xl font-bold mb-4">報名成功！</h2>
            <p className="mb-4">我們已收到您的報名資訊</p>
            <p className="text-gray-600 mb-4">
              請於 24 小時內完成付款程序，以確保您的報名資格
            </p>
            <Button 
              onClick={() => setIsSubmitted(false)}
              className="mt-4"
            >
              返回表單
            </Button>
          </CardContent>
        </Card>
      );
    }

    return (
      <Card className="w-full max-w-md mx-auto mt-10">
        <CardHeader>
          <CardTitle className="text-2xl font-bold text-center">活動報名表單</CardTitle>
        </CardHeader>
        <CardContent>
          <form onSubmit={handleSubmit} className="space-y-6">
            <div className="space-y-2">
              <Label htmlFor="name">姓名</Label>
              <Input
                id="name"
                value={formState.name}
                onChange={(e) => setFormState({...formState, name: e.target.value})}
                placeholder="請輸入您的姓名"
                className={errors.name ? "border-red-500" : ""}
              />
              {errors.name && <p className="text-red-500 text-sm">{errors.name}</p>}
            </div>

            <div className="space-y-2">
              <Label htmlFor="phone">手機號碼</Label>
              <Input
                id="phone"
                value={formState.phone}
                onChange={(e) => setFormState({...formState, phone: e.target.value})}
                placeholder="請輸入您的手機號碼"
                className={errors.phone ? "border-red-500" : ""}
              />
              {errors.phone && <p className="text-red-500 text-sm">{errors.phone}</p>}
            </div>

            <div className="space-y-2">
              <Label htmlFor="email">Email</Label>
              <Input
                id="email"
                type="email"
                value={formState.email}
                onChange={(e) => setFormState({...formState, email: e.target.value})}
                placeholder="請輸入您的 Email"
                className={errors.email ? "border-red-500" : ""}
              />
              {errors.email && <p className="text-red-500 text-sm">{errors.email}</p>}
            </div>

            <div className="space-y-2">
              <Label htmlFor="dietary">飲食習慣</Label>
              <Select
                value={formState.dietary}
                onValueChange={(value) => setFormState({...formState, dietary: value})}
              >
                <SelectTrigger className={errors.dietary ? "border-red-500" : ""}>
                  <SelectValue placeholder="請選擇飲食習慣" />
                </SelectTrigger>
                <SelectContent>
                  <SelectItem value="normal">葷食</SelectItem>
                  <SelectItem value="vegetarian">素食</SelectItem>
                  <SelectItem value="vegan">純素</SelectItem>
                </SelectContent>
              </Select>
              {errors.dietary && <p className="text-red-500 text-sm">{errors.dietary}</p>}
            </div>

            <Button type="submit" className="w-full">
              提交報名
            </Button>
          </form>
        </CardContent>
      </Card>
    );
  };

  export default RegistrationForm;
