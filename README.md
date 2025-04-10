import React from "react";
import { MoveUpRight } from "lucide-react"; // đảm bảo cài lucide-react
import { Button } from "@/components/ui/button"; // hoặc thay bằng <button> nếu không có component Button

const SietEoPage = () => {
  return (
    <div className="bg-gradient-to-b from-pink-100 to-white min-h-screen py-12 px-4 md:px-12">
      <div className="max-w-5xl mx-auto grid gap-12">

        {/* BUỔI 2 + 3 */}
        <div className="grid md:grid-cols-2 gap-6">
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
            <button type="submit" className="bg-pink-500 hover:bg-pink-600 text-white py-4 text-lg rounded-2xl flex items-center justify-center gap-2">
              Gửi đăng ký <MoveUpRight />
            </button>
          </form>
        </div>

        {/* CALL TO ACTION */}
        <div className="text-center">
          <h2 className="text-3xl font-bold mb-4">Sẵn sàng Siết Eo Không Stress?</h2>
          <p className="mb-6 text-lg">
            Đặt trước ngay hôm nay để nhận ưu đãi + bộ quà tặng giới hạn!
          </p>
          <button className="bg-pink-500 hover:bg-pink-600 text-white text-lg px-8 py-6 rounded-2xl flex items-center justify-center gap-2">
            Đăng Ký Ngay <MoveUpRight />
          </button>
        </div>

      </div>
    </div>
  );
};

export default SietEoPage;
