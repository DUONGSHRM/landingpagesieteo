# landingpagesieteo
Chương trình siết eo với Latex hè 2025
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { CheckCircle, Gift, Video, NotebookPen, MoveUpRight, Clock } from "lucide-react";

export default function LandingPage() {
  return (
    <div className="bg-[#fef8f4] min-h-screen py-10 px-4 md:px-20 text-[#2e1e17]">
      <div className="max-w-5xl mx-auto grid gap-10">
        <h1 className="text-4xl md:text-5xl font-bold leading-tight">
          Gói Coaching Mastery: Siết Eo Làm Chủ Vóc Dáng
        </h1>
        <p className="text-lg md:text-xl">
          Hành trình 3 buổi coaching + latex định hình + meal plan + video hướng dẫn giúp bạn sở hữu vòng eo săn gọn mà không cần ép xác.
        </p>

        {/* COUNTDOWN */}
        <div className="bg-pink-100 text-center p-4 rounded-xl shadow-md">
          <h3 className="text-xl font-semibold mb-2">Ưu đãi đặc biệt chỉ còn:</h3>
          <p className="text-3xl font-bold text-pink-600">02 ngày 12 giờ 45 phút</p>
        </div>

        <Card className="bg-white shadow-xl rounded-2xl p-6">
          <CardContent className="grid gap-6">
            <div className="grid md:grid-cols-2 gap-6">
              <div>
                <h2 className="text-2xl font-semibold mb-4">Bạn sẽ nhận được:</h2>
                <ul className="space-y-3">
                  <li className="flex items-start gap-2">
                    <CheckCircle className="text-pink-500" />
                    3 buổi coaching online theo nhóm
                  </li>
                  <li className="flex items-start gap-2">
                    <Gift className="text-pink-500" />
                    1 Latex định hình cao cấp (chọn size)
                  </li>
                  <li className="flex items-start gap-2">
                    <NotebookPen className="text-pink-500" />
                    Sổ tay Eo Gọn A5 + Printable meal plan & tracker
                  </li>
                  <li className="flex items-start gap-2">
                    <Video className="text-pink-500" />
                    Video tập luyện 21 ngày + playlist hàng ngày
                  </li>
                </ul>
              </div>
              <img
                src="/images/latex-kit-preview.png"
                alt="Latex Kit"
                className="rounded-xl w-full shadow-md"
              />
            </div>
          </CardContent>
        </Card>

        {/* SECTION COACHING DETAILS */}
        <div className="grid gap-6">
          <h2 className="text-3xl font-bold">Chi tiết 3 buổi Coaching</h2>
          <div className="bg-white p-6 rounded-xl shadow">
            <h3 className="text-xl font-semibold mb-2">Buổi 1: Siết mà không stress</h3>
            <p>Giới thiệu cách dùng latex đúng cách + detox nhẹ + đặt mục tiêu cá nhân hóa.</p>
          </div>
          <div className="bg-white p-6 rounded-xl shadow">
            <h3 className="text-xl font-semibold mb-2">Buổi 2: Thở đúng, eo gọn</h3>
            <p>Kỹ thuật hơi thở đánh thức bụng dưới + tập core nhẹ nhàng với latex.</p>
          </div>
          <div className="bg-white p-6 rounded-xl shadow">
            <h3 className="text-xl font-semibold mb-2">Buổi 3: Body Ready – Mind Steady</h3>
            <p>Đánh giá kết quả + tư duy duy trì vóc dáng lâu dài và tự tin mặc đồ đẹp.</p>
          </div>
        </div>

        {/* TESTIMONIAL */}
        <div className="grid gap-6">
          <h2 className="text-3xl font-bold">Khách Hàng Nói Gì?</h2>
          <div className="grid md:grid-cols-2 gap-4">
            <div className="bg-white p-4 rounded-xl shadow">
              <p>“Mới tuần đầu mà bụng đã gọn rõ luôn! Latex mặc dễ chịu, không bị khó thở. Em mê luôn playlist tập nhẹ mỗi sáng.”</p>
              <p className="mt-2 font-semibold">– Lan Anh, 31 tuổi</p>
            </div>
            <div className="bg-white p-4 rounded-xl shadow">
              <p>“Đi làm văn phòng cả ngày, nhờ chị Dương hướng dẫn mà biết cách siết nhẹ nhàng, không ép xác mà vẫn có eo.”</p>
              <p className="mt-2 font-semibold">– Thu Hương, HR Executive</p>
            </div>
          </div>
        </div>

        {/* SIGNUP FORM */}
        <div className="bg-white p-6 rounded-xl shadow grid gap-4">
          <h2 className="text-3xl font-bold">Đăng ký ngay</h2>
          <p className="text-lg">Điền thông tin để giữ suất và nhận bộ latex kit</p>
          <form className="grid gap-4">
            <input type="text" placeholder="Họ và tên" className="border p-3 rounded-xl" />
            <input type="email" placeholder="Email" className="border p-3 rounded-xl" />
            <input type="tel" placeholder="Số điện thoại" className="border p-3 rounded-xl" />
            <Button className="bg-pink-500 hover:bg-pink-600 text-white py-4 text-lg rounded-2xl">
              Gửi đăng ký <MoveUpRight className="inline ml-2" />
            </Button>
          </form>
        </div>

        <div className="text-center">
          <h2 className="text-3xl font-bold mb-4">Sẵn sàng Siết Eo Không Stress?</h2>
          <p className="mb-6 text-lg">
            Đặt trước ngay hôm nay để nhận ưu đãi + bộ quà tặng giới hạn!
          </p>
          <Button className="bg-pink-500 hover:bg-pink-600 text-white text-lg px-8 py-6 rounded-2xl">
            Đăng Ký Ngay <MoveUpRight className="inline ml-2" />
          </Button>
        </div>
      </div>
    </div>
  );
}
